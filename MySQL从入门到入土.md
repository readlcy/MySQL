# MySQL从入门到入土

## 1 SQL

**约定：**

1. 中括号内的语句为可选语句，可加可不加。
2. SQL语句不区分大小写，但为了与其他部分做区分，此处SQL语句关键字均为为大写。



### 1.2 DDL

#### 1.2.1 数据库操作

##### 查看所有数据库

```sql
SHOW DATABASES;
```



##### 查询当前所处数据库

```sql
SELECT DATABASE();
```



##### 创建数据库

```sql
CREATE DATABASE 数据库名;
```



##### 访问数据库

```sql
USE 数据库名;
```



##### 删除数据库

```sql
DROP DATABASE 数据库名;
```

#### 1.2.2 表操作

查询当前数据库所有表

```sql
SHOW TABLES;
```



查询表结构

```sql
DESC 表名;
```



查询指定表的建表语句

```sql
SHOW CREATE TABLE 表名;
```



创建表

```sql
CREATE TABLE 表名(
字段1 字段1类型[COMMENT 字段1注释],
字段2 字段2类型[COMMENT 字段2注释],
字段3 字段3类型[COMMENT 字段3注释],
...
字段n 字段n类型[COMMENT 字段n注释]
)[COMMENT 表注释];
```

**注意：最后一个字段末尾不添加逗号。**

数据类型——数值

| 类型          | 大小    | 有符号(SIGNED)范围                                    | 无符号(UNSIGNED)范围                                      | 描述               |
| ------------- | ------- | ----------------------------------------------------- | --------------------------------------------------------- | ------------------ |
| TINYINT       | 1 byte  | (-128, 127)                                           | (0，255)                                                  | 小整数值           |
| SMALLINT      | 2 bytes | (-32768, 32767)                                       | (0，65535)                                                | 大整数值           |
| MEDIUMINT     | 3 bytes | (-8388608, 8388607)                                   | (0，16777215)                                             | 大整数值           |
| INT或 INTEGER | 4 bytes | (-2147483648, 2147483647)                             | (0，4294967295)                                           | 大整数值           |
| BIGINT        | 8 bytes | (-2~63, 2~63-1)                                       | (0，2^64-1)                                               | 极大整数值         |
| FLOAT         | 4 bytes | (-3.402823466 E+38, 3.402823466351 E+38)              | 0 和 (1.175494351 E-38，3.402823466 E+38)                 | 单精度浮点数值     |
| DOUBLE        | 8 bytes | (-1.7976931348623157 E+308, 1.7976931348623157 E+308) | 0 和 (2.2250738585072014 E-308，1.7976931348623157 E+308) | 双精度浮点数值     |
| DECIMAL       |         | 依赖于M(精度)和D(标度)的值                            | 依赖于M(精度)和D(标度)的值                                | 小数值(精确定点数) |

精度：整个数值的长度。

标度：小数部分的长度。

列如：123.45的精度为5，标度为2。

数据类型——字符串

| 类型       | 大小                | 描述                         |
| ---------- | ------------------- | ---------------------------- |
| CHAR       | 0-255 bytes         | 定长字符串                   |
| VARCHAR    | 0-65535 bytes       | 变长字符串                   |
| TINYBLOB   | 0-255 bytes         | 不超过255个字符的二进制数据  |
| TINYTEXT   | 0-255 bytes         | 短文本字符串                 |
| BLOB       | 0-65535 bytes       | 二进制形式的长文本数据       |
| TEXT       | 0-65 535 bytes      | 长文本数据                   |
| MEDIUMBLOB | 0-16777215 bytes    | 二进制形式的中等长度文本数据 |
| MEDIUMTEXT | 0-16777215 bytes    | 中等长度文本数据             |
| LONGBLOB   | 0-4294967295 bytes  | 二进制形式的极大文本数据     |
| LONGTEXT   | 0-4 294967295 bytes | 极大文本数据                 |

数据类型——日期

| 类型      | 大小 | 范围                                       | 格式                | 描述                     |
| --------- | ---- | ------------------------------------------ | ------------------- | ------------------------ |
| DATE      | 3    | 1000-01-01 至 9999-12-31                   | YYYY-MM-DD          | 日期值                   |
| TIME      | 3    | -838:59:59 至 838:59:59                    | HH:MM:SS            | 时间值或持续时间         |
| YEAR      | 1    | 1901 至 2155                               | YYYY                | 年份值                   |
| DATETIME  | 8    | 1000-01-01 00:00:00 至 9999-12-31 23:59:59 | YYYY-MM-DD HH:MM:SS | 混合日期和时间值         |
| TIMESTAMP | 4    | 1970-01-01 00:00:01 至 2038-01-19 03:14:07 | YYYY-MM-DD HH:MM:SS | 混合日期和时间值，时间戳 |





### 1.3 DML

#### 添加数据

```sql
INSERT INTO 表名(字段1, 字段2, ...) VALUES(值1, 值2, ...) [, (值1, 值2, ...) ...];
```



#### 修改数据

```sql
UPDATE 表名 SET 字段1 = 值1, 字段2 = 值2, ... [WHERE 条件];
```



#### 删除数据

```sql
DELETE FROM 表名 [WHERE 条件];
```



### 1.4 DQL

```sql
SELECT
	字段列表
FROM
	表名
WHERE
	条件列表
GROUP BY
	分组字段列表
HAVING
	分组后条件列表
ORDER BY
	排序字段列表
LIMIT
	分页参数
```







聚合函数

| 函数  | 功能     |
| ----- | -------- |
| count | 统计数量 |
| max   | 最大值   |
| min   | 最小值   |
| avg   | 平均值   |
| sum   | 求和     |



### 1.5 DCL 

权限控制

| 权限                | 说明               |
| :------------------ | :----------------- |
| ALL, ALL PRIVILEGES | 所有权限           |
| SELECT              | 查询数据           |
| INSERT              | 插入数据           |
| UPDATE              | 修改数据           |
| DELETE              | 删除数据           |
| ALTER               | 修改表             |
| DROP                | 删除数据库/表/视图 |
| CREATE              | 创建数据库/表      |





## 2 函数

### 2.1 字符串函数

| 函数                     | 功能                                                      |
| ------------------------ | --------------------------------------------------------- |
| CONCAT(S1,S2,..Sn)       | 字符串拼接，将S1，S2，…..Sn拼接成一个字符串               |
| LOWER(str)               | 将字符串str全部转为小写                                   |
| UPPER(str)               | 将字符串str全部转为大写                                   |
| LPAD(str,n,pad)          | 左填充，用字符串pad对str的左边进行填充，达到n个字符串长度 |
| RPAD(str,n,pad)          | 右填充，用字符串pad对str的右边进行填充，达到n个字符串长度 |
| TRIM(str)                | 去掉字符串头部和尾部的空格                                |
| SUBSTRING(str,start,len) | 返回从字符串str从start位置起的len个长度的字符串           |

### 2.2 数值函数

| 函数       | 功能                               |
| ---------- | ---------------------------------- |
| CEIL(x)    | 向上取整                           |
| FLOOR(x)   | 向下取整                           |
| MOD(x,y)   | 返回x/y的模                        |
| RAND()     | 返回0~1内的随机数                  |
| ROUND(x,y) | 求参数x的四舍五入的值，保留y位小数 |

### 2.3 日期函数

| 函数                               | 功能                                              |
| ---------------------------------- | ------------------------------------------------- |
| CURDATE()                          | 返回当前日期                                      |
| CURTIME()                          | 返回当前时间                                      |
| NOW()                              | 返回当前日期和时间                                |
| YEAR(date)                         | 获取指定date的年份                                |
| MONTH(date)                        | 获取指定date的月份                                |
| DAY(date)                          | 获取指定date的日期                                |
| DATE_ADD(date, INTERVAL expr type) | 返回一个日期/时间值加上一个时间间隔expr后的时间值 |
| DATEDIFF(date1,date2)              | 返回起始时间date1 和 结束时间date2之间的天数      |

### 2.4 流程函数

| 函数                                                         | 功能                                                   |
| ------------------------------------------------------------ | ------------------------------------------------------ |
| IF(value ,t, f)                                              | 如果value为true，则返回t，否则返回f                    |
| IFNULL(value1 , value2)                                      | 如果valuel不为空，返回value1，否则返回value2           |
| CASE WHEN [vall ] THEN [res] ... ELSE[default] END           | 如果vall为true，返回res1l，. 否则返回default默认值     |
| CASE [expr ]  WHEN [val1 ] THEN [res1] ... ELSE[ default ]  END | 如果expr的值等于vall，返回res1，.否则返回default默认值 |





## 3 约束

| 约束     | 描述                                                     | 关键字      |
| -------- | -------------------------------------------------------- | ----------- |
| 非空约束 | 限制该字段的数据不能为null                               | NOT NULL    |
| 唯一约束 | 保证该字段的所有数据都是唯一、不重复的                   | UNIQUE      |
| 主键约束 | 主键是一行数据的唯一标识，要求非空且唯一                 | PRIMARY KEY |
| 默认约束 | 保存数据时，如果未指定该字段的值，则采用默认值           | DEFAULT     |
| 检查约束 | 保证字段值满足某一个条件                                 | CHECK       |
| 外键约束 | 用来让两张表的数据之间建立连接，保证数据的一致性和完整性 | FOREIGN KEY |

### 外键约束

#### 添加外键

```sql
CREATE TABLE 表名(
字段名 数据类型,
...
[CONSTRAINT] 外键名称  FOREIGN KEY(外键字段名) REFERENCES 主表(主表列名)
);
```

```
ALTER TABLE 表名 ADD CONSTRAINT 外键名称 FOREIGN KEY(外键字段名）REFERENCES 主表(主表列名);
```

注意：添加外键时的指向的主表字段一定要是主键

<img src="D:\Typora\save\MySQL\assets\添加外键代码.png"  />

```sql
SELECT * FROM table_1 WHERE ID < 4 AND ID > 1 LIMIT 0 ,2;

CREATE TABLE STUDENT(
    ID INT PRIMARY KEY ,
    NAME VARCHAR(4) UNIQUE,
    CLASS INT DEFAULT 1,
    SCHOOLID INT,
    CONSTRAINT SCHOOL_KEY FOREIGN KEY (SCHOOLID) REFERENCES SCHOOL(ID)
);

CREATE TABLE SCHOOL(
    ID INT,
    NAME VARCHAR(5)
);


INSERT INTO SCHOOL VALUES (1,'任远'),(2,'一中'),(3,'二中'),(4,'玉树');

INSERT INTO STUDENT VALUES (1, '张三', 1,1),(2,'李四',2, '2'),
                           (3,'王五',1,1),(4,'麻子',1,1),

                           (5,'丁一', 6,4),(6,'牛二',5,3);
```



![](D:\Typora\save\MySQL\assets\添加外键的表1.png)

![](D:\Typora\save\MySQL\assets\添加外键的表2.png)



#### 删除外键

```
ALTER TABLE 表名 DROP FOREIGN KEY 外键名称;
```

删除更新行为

| 行为        | 说明                                                         |
| ----------- | ------------------------------------------------------------ |
| NO ACTION   | 当在父表中删除/更新对应记录时，首先检查该记录是否有对应外键，如果有则不允许删除/更新。 (与 RESTRICT一致) |
| RESTRICT    | 当在父表中删除/更新对应记录时，首先检查该记录是否有对应外键，如果有则不允许删除/更新。 (与 NO ACTION 一致) |
| CASCADE     | 当在父表中删除/更新对应记录时，首先检查该记录是否有对应外键，如果有，则也删除/更新外键在子表中的记录。 |
| SET NULL    | 当在父表中删除对应记录时，首先检查该记录是否有对应外键，如果有则设置子表中该外键值为null（这就要求该外键允许取nulI）。 |
| SET DEFAULT | 父表有变更时，子表将外键列设置成一个默认的值 (Innodb不支持)  |



## 4  连接查询

### 4.1 连接查询-内连接

**隐式内连接**

```sql
SELECT 字段列表 FROM 表1, 表2 WHERE条件 ...;
```

**显式内连接**

```sql
SELECT 字段列表 FROM 表1 [INNER] JOIN 表2 ON 连接条件 ..;
```

内连接查询的是两张表交集的部分

![](D:\Typora\save\MySQL\assets\连接查询.png)

### 连接查询-外连接

**左外连接**

```sql
SELECT 字段列表 FROM 表A LEFT [OUTER] JOIN 表B ON 条件 ...;
```

![](D:\Typora\save\MySQL\assets\左外连接.png)

相当于查询表A(左表)的所有数据，包含表A和表B交集部分的数据

注意最后一行数据，

**右外连接**

```sql
SELECT 字段列表 FROM 表A RIGHT [OUTER] JOIN 表B ON 条件 ...;
```

相当于查询表B(右表)的所有数据，包含表A和表B交集部分的数据

### 连接查询-自连接

自连接查询语法：

```sql
SELECT 字段列表 FROM 表A 别名A JOIN 表A  别名B ON 条件...
```

自连接查询，可以是内连接查询，也可以是外连接查询。

### 联合查询-union，unionall

对于union查询，就是把多次查询的结果合并起来，形成一个新的查询结果集。

```sql
SELECT 字段列表 FROM 表A...
UNION [ALL]
SELECT 字段列表 FROM 表B...;
```

对于联合查询的多张表的列数必须保持一致，字段类型也需要保持一致。

unionall会将全部的数据直接合并在一起，union会对合并之后的数据去重。

### 子查询

概念：SQL语句中嵌套SELECT语句，称为嵌套查询，又称子查询。

```sql
SELECT * FROM tl WHERE column1 = (SELECT column1 FROM t2);
```

**子查询外部的语句可以是INSERT/UPDATE/DELETE／SELECT的任何一个。**

根据子查询结果不同，分为：

- 标量子查询 (子查询结果为单个值)
- 列子查询(子查询结果为一列)
- 行子查询(子查询结果为一行)
- 表子查询(子查询结果为多行多列)

根据子查询位置，分为：WHERE之后、FROM之后、SELECT 之后。

#### 标量子查询

子查询返回的结果是单个值（数字、字符串、日期等），最简单的形式，这种子查询成为标量子查询。

常用的操作符：=  <>  >   >=   <  <=

示例：查询来自任远的学生信息（学校信息表和学生信息表见上）

此例可以分两个步骤来做，首先查询学校信息表中任远中学的编号：

![](D:\Typora\save\MySQL\assets\标量子查询示例1.png)

结果返回1，这时再查询学校编号在学生信息表中对应的学生：

![](D:\Typora\save\MySQL\assets\标量子查询示例2.png)

而利用标量子查询可以用一行代码解决这个问题，标量子查询的关键在于把代码看出一个值，如步骤一代码返回值为是学校编号，那就把这行代码看作是学校编号，同理，在后页面的表子查询中，代码返回一张表，那就可以把代码当成一张表在其它代码中使用。

注意：使用时要加括号

![](D:\Typora\save\MySQL\assets\标量子查询示例3.png)

#### 列子查询

子查询返回的结果是一列（可以是多行），这种子查询称为列子查询。

常用的操作符：IN、NOTIN、ANY、SOME、ALL

| 操作符 | 描述                                   |
| ------ | -------------------------------------- |
| IN     | 在指定的集合范围之内，多选一           |
| NOT IN | 不在指定的集合范围之内                 |
| ANY    | 子查询返回列表中，有任意一个满足即可   |
| SOME   | 与ANY等同，使用SOME的地方都可以使用ANY |
| ALL    | 子查询返回列表的所有值都必须满足       |

#### 行子查询

子查询返回的结果是一行（可以是多列），这种子查询称为行子查询。

常用的操作符：=、<>、IN、NOT IN

补充知识点：

```sql
SELECT * FROM 表A WHERE 字段1 = 值1 AND 字段2 = 值2; 
```

```sql
SELECT * FROM 表A WHERE (字段1, 字段2) = (值1, 值2); 
```

两种写法等效

#### 表子查询

子查询返回的结果是多行多列，这种子查询称为表子查询

常用的操作符：IN

补充知识点：

```sql
SELECT * FROM 表A WHERE (字段1, 字段2) IN (表b); 
```

表b中的字段与括号内字段相同，可以查询到表a中满足两字段等于表b中任何一行数据的数据



## 事务

### 事务操作

#### 查看/设置事务提交方式

```sql
SELECT @@autocommit ;
SET @@autocommit = 0;
```

#### 开启事务

```sql
START TRANSACTION 或 BEGIN ;
```

#### 提交事务

```sql
COMMIT ;
```

#### 回滚事务

```sql
ROLLBACK ;
```

### <font color='red'>事务四大特性</font>

**原子性**（<font color='red'>A</font>tomicity）：事务是不可分割的最小操作单元，要么全部成功，要么全部失败。

**一致性**（<font color='red'>C</font>onsistency）：事务完成时，必须使所有的数据都保持一致状态。

**隔离性**（<font color='red'>I</font>solation）：数据库系统提供的隔离机制，保证事务在不受外部并发操作影响的独立环境下运行。

**持久性**（<font color='red'>D</font>urability）：事务一旦提交或回滚，它对数据库中的数据的改变就是永久的。

### 并发事务问题

| 问题       | 描述                                                         |
| ---------- | ------------------------------------------------------------ |
| 脏读       | 一个事务读到另外一个事务还没有提交的数据。                   |
| 不可重复读 | 一个事务先后读取同一条记录，但两次读取的数据不同，称之为不可重复读。 |
| 幻读       | 一个事务按照条件查询数据时，没有对应的数据行，但是在插入数据时，又发现这行数据已经存在，好像出现了"幻影"。 |

### 事务隔离级别

| 隔离级别              | 脏读 | 不可重复读 | 幻读 |
| --------------------- | ---- | ---------- | ---- |
| Read uncommitted      | √    | √          | √    |
| Read committed        | ×    | √          | √    |
| Repeatable Read(默认) | ×    | ×          | √    |
| Serializable          | ×    | ×          | ×    |

#### 查看事务隔离级别

```sql
SELECT @@TRANSACTION_ISOLATION;
```

#### 设置事务隔离级别

```sql
SET [SESSION | GLOBAL] TRANSACTION ISOLATION LEVEL { READ UNCOMMITTED | READ COMMITTED | REPEATABLE READ | SERIALIZABLE } 
```

注意：事务隔离级别越高。数据安全性越好，但同时性能也会越差
