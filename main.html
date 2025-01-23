<h1>MySQL从入门到入土——入门篇</h1>
<h2>1 SQL</h2>
<p><strong>约定：</strong></p>
<ol>
<li>中括号内的语句为可选语句，可加可不加。</li>
<li>SQL语句不区分大小写，但为了与其他部分做区分，此处SQL语句关键字均为为大写。</li>

</ol>
<h3>1.1 通用知识</h3>
<h4>1.1.1 SQL通用语法</h4>
<p>1.SQL语句可以单行或多行书写，以分号结尾。</p>
<p>2.SQL语句可以使用空格/缩进来增强语句的可读性。</p>
<p>3.MySQL数据库的SQL语句不区分大小写，关键字建议使用大写。</p>
<p>4.注释：</p>
<ul>
<li>单行注释：-- 注释内容 或 #注释内容(MySQL特有)</li>

</ul>
<ul>
<li>多行注释：/*注释内容*/</li>

</ul>
<h4>1.1.2 SQL分类</h4>
<figure class='table-figure'><table>
<thead>
<tr><th>分类</th><th>全称</th><th>说明</th></tr></thead>
<tbody><tr><td>DDL</td><td> Data Definition Language</td><td>数据定义语言，用来定义数据库对象(数据库，表，字段)</td></tr><tr><td>DML</td><td> Data Manipulation Language</td><td>数据操作语言，用来对数据库表中的数据进行增删改</td></tr><tr><td>DQL</td><td> Data Query Language</td><td>数据查询语言，用来查询数据库中表的记录</td></tr><tr><td>DCL</td><td> Data Control Language</td><td>数据控制语言，用来创建数据库用户、控制数据库的访问权限</td></tr></tbody>
</table></figure>
<p>&nbsp;</p>
<h3>1.2 DDL</h3>
<h4>1.2.1 数据库操作</h4>
<p>查看所有数据库</p>
<pre><code class='language-sql' lang='sql'>SHOW DATABASES;
</code></pre>
<p>&nbsp;</p>
<p>查询当前所处数据库</p>
<pre><code class='language-sql' lang='sql'>SELECT DATABASE();
</code></pre>
<p>&nbsp;</p>
<p>创建数据库</p>
<pre><code class='language-sql' lang='sql'>CREATE DATABASE 数据库名;
</code></pre>
<p>&nbsp;</p>
<p>访问数据库</p>
<pre><code class='language-sql' lang='sql'>USE 数据库名;
</code></pre>
<p>&nbsp;</p>
<p>删除数据库</p>
<pre><code class='language-sql' lang='sql'>DROP DATABASE 数据库名;
</code></pre>
<p>&nbsp;</p>
<h4>1.2.2 表操作</h4>
<h5>1.2.2.1 表操作-查询</h5>
<p>查询当前数据库所有表</p>
<pre><code class='language-sql' lang='sql'>SHOW TABLES;
</code></pre>
<p>&nbsp;</p>
<p>查询表结构</p>
<pre><code class='language-sql' lang='sql'>DESC 表名;
</code></pre>
<p>&nbsp;</p>
<p>查询指定表的建表语句</p>
<pre><code class='language-sql' lang='sql'>SHOW CREATE TABLE 表名;
</code></pre>
<p>&nbsp;</p>
<h5>1.2.2.2 表操作-修改</h5>
<p>添加字段</p>
<pre><code>ALTER TABLE 表名 ADD 字段名 类型(长度) [COMMENT 注释] [约束];
</code></pre>
<p>&nbsp;</p>
<p>修改数据类型</p>
<pre><code>ALTER TABLE 表名 MODIFY 字段名 新数据类型(长度);
</code></pre>
<p>&nbsp;</p>
<p>修改字段名和字段类型</p>
<pre><code>ALTER TABLE 表名 CHANGEI 旧字段名 新字段名 类型(长度) [COMMENT 注释] [约束];
</code></pre>
<p>&nbsp;</p>
<h5>1.2.1.3 表操作-删除</h5>
<p>删除字段</p>
<pre><code>ALTER TABLE 表名 DROP 字段名;
</code></pre>
<p>&nbsp;</p>
<p>删除表</p>
<pre><code>DROP TABLE [IF EXISTS] 表名;
</code></pre>
<p>&nbsp;</p>
<p>删除指定表，并重新创建该表</p>
<pre><code>TRUNCATE TABLE 表名
</code></pre>
<p>&nbsp;</p>
<p>创建表</p>
<pre><code class='language-sql' lang='sql'>CREATE TABLE 表名(
字段1 字段1类型[COMMENT 字段1注释],
字段2 字段2类型[COMMENT 字段2注释],
字段3 字段3类型[COMMENT 字段3注释],
...
字段n 字段n类型[COMMENT 字段n注释]
)[COMMENT 表注释];
</code></pre>
<p><strong>注意：最后一个字段末尾不添加逗号。</strong></p>
<p>&nbsp;</p>
<h4>1.2.3 数据类型</h4>
<h5>1.2.3.1 数据类型——数值</h5>
<figure class='table-figure'><table>
<thead>
<tr><th>类型</th><th>大小</th><th>有符号(SIGNED)范围</th><th>无符号(UNSIGNED)范围</th><th>描述</th></tr></thead>
<tbody><tr><td>TINYINT</td><td>1 byte</td><td>(-128, 127)</td><td>(0，255)</td><td>小整数值</td></tr><tr><td>SMALLINT</td><td>2 bytes</td><td>(-32768, 32767)</td><td>(0，65535)</td><td>大整数值</td></tr><tr><td>MEDIUMINT</td><td>3 bytes</td><td>(-8388608, 8388607)</td><td>(0，16777215)</td><td>大整数值</td></tr><tr><td>INT或 INTEGER</td><td>4 bytes</td><td>(-2147483648, 2147483647)</td><td>(0，4294967295)</td><td>大整数值</td></tr><tr><td>BIGINT</td><td>8 bytes</td><td>(-2~63, 2~63-1)</td><td>(0，2^64-1)</td><td>极大整数值</td></tr><tr><td>FLOAT</td><td>4 bytes</td><td>(-3.402823466 E+38, 3.402823466351 E+38)</td><td>0 和 (1.175494351 E-38，3.402823466 E+38)</td><td>单精度浮点数值</td></tr><tr><td>DOUBLE</td><td>8 bytes</td><td>(-1.7976931348623157 E+308, 1.7976931348623157 E+308)</td><td>0 和 (2.2250738585072014 E-308，1.7976931348623157 E+308)</td><td>双精度浮点数值</td></tr><tr><td>DECIMAL</td><td>&nbsp;</td><td>依赖于M(精度)和D(标度)的值</td><td>依赖于M(精度)和D(标度)的值</td><td>小数值(精确定点数)</td></tr></tbody>
</table></figure>
<p>精度：整个数值的长度。</p>
<p>标度：小数部分的长度。</p>
<p>列如：123.45的精度为5，标度为2。</p>
<h5>1.2.3.2 数据类型——字符串</h5>
<figure class='table-figure'><table>
<thead>
<tr><th>类型</th><th>大小</th><th>描述</th></tr></thead>
<tbody><tr><td>CHAR</td><td>0-255 bytes</td><td>定长字符串</td></tr><tr><td>VARCHAR</td><td>0-65535 bytes</td><td>变长字符串</td></tr><tr><td>TINYBLOB</td><td>0-255 bytes</td><td>不超过255个字符的二进制数据</td></tr><tr><td>TINYTEXT</td><td>0-255 bytes</td><td>短文本字符串</td></tr><tr><td>BLOB</td><td>0-65535 bytes</td><td>二进制形式的长文本数据</td></tr><tr><td>TEXT</td><td>0-65 535 bytes</td><td>长文本数据</td></tr><tr><td>MEDIUMBLOB</td><td>0-16777215 bytes</td><td>二进制形式的中等长度文本数据</td></tr><tr><td>MEDIUMTEXT</td><td>0-16777215 bytes</td><td>中等长度文本数据</td></tr><tr><td>LONGBLOB</td><td>0-4294967295 bytes</td><td>二进制形式的极大文本数据</td></tr><tr><td>LONGTEXT</td><td>0-4 294967295 bytes</td><td>极大文本数据</td></tr></tbody>
</table></figure>
<h5>1.2.3.3 数据类型——日期</h5>
<figure class='table-figure'><table>
<thead>
<tr><th>类型</th><th>大小</th><th>范围</th><th>格式</th><th>描述</th></tr></thead>
<tbody><tr><td>DATE</td><td>3</td><td>1000-01-01 至 9999-12-31</td><td>YYYY-MM-DD</td><td>日期值</td></tr><tr><td>TIME</td><td>3</td><td>-838:59:59 至 838:59:59</td><td>HH:MM:SS</td><td>时间值或持续时间</td></tr><tr><td>YEAR</td><td>1</td><td>1901 至 2155</td><td>YYYY</td><td>年份值</td></tr><tr><td>DATETIME</td><td>8</td><td>1000-01-01 00:00:00 至 9999-12-31 23:59:59</td><td>YYYY-MM-DD HH:MM:SS</td><td>混合日期和时间值</td></tr><tr><td>TIMESTAMP</td><td>4</td><td>1970-01-01 00:00:01 至 2038-01-19 03:14:07</td><td>YYYY-MM-DD HH:MM:SS</td><td>混合日期和时间值，时间戳</td></tr></tbody>
</table></figure>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>1.3 DML</h3>
<h4>添加数据</h4>
<pre><code class='language-sql' lang='sql'>INSERT INTO 表名(字段1, 字段2, ...) VALUES(值1, 值2, ...) [, (值1, 值2, ...) ...];
</code></pre>
<p>&nbsp;</p>
<h4>修改数据</h4>
<pre><code class='language-sql' lang='sql'>UPDATE 表名 SET 字段1 = 值1, 字段2 = 值2, ... [WHERE 条件];
</code></pre>
<p>&nbsp;</p>
<h4>删除数据</h4>
<pre><code class='language-sql' lang='sql'>DELETE FROM 表名 [WHERE 条件];
</code></pre>
<p>&nbsp;</p>
<h3>1.4 DQL</h3>
<pre><code class='language-sql' lang='sql'>SELECT
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
</code></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>聚合函数</p>
<figure class='table-figure'><table>
<thead>
<tr><th>函数</th><th>功能</th></tr></thead>
<tbody><tr><td>count</td><td>统计数量</td></tr><tr><td>max</td><td>最大值</td></tr><tr><td>min</td><td>最小值</td></tr><tr><td>avg</td><td>平均值</td></tr><tr><td>sum</td><td>求和</td></tr></tbody>
</table></figure>
<p>&nbsp;</p>
<h3>1.5 DCL </h3>
<p>权限控制</p>
<figure class='table-figure'><table>
<thead>
<tr><th style='text-align:left;' >权限</th><th style='text-align:left;' >说明</th></tr></thead>
<tbody><tr><td style='text-align:left;' >ALL, ALL PRIVILEGES</td><td style='text-align:left;' >所有权限</td></tr><tr><td style='text-align:left;' >SELECT</td><td style='text-align:left;' >查询数据</td></tr><tr><td style='text-align:left;' >INSERT</td><td style='text-align:left;' >插入数据</td></tr><tr><td style='text-align:left;' >UPDATE</td><td style='text-align:left;' >修改数据</td></tr><tr><td style='text-align:left;' >DELETE</td><td style='text-align:left;' >删除数据</td></tr><tr><td style='text-align:left;' >ALTER</td><td style='text-align:left;' >修改表</td></tr><tr><td style='text-align:left;' >DROP</td><td style='text-align:left;' >删除数据库/表/视图</td></tr><tr><td style='text-align:left;' >CREATE</td><td style='text-align:left;' >创建数据库/表</td></tr></tbody>
</table></figure>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h2>2 函数</h2>
<h3>2.1 字符串函数</h3>
<figure class='table-figure'><table>
<thead>
<tr><th>函数</th><th>功能</th></tr></thead>
<tbody><tr><td>CONCAT(S1,S2,..Sn)</td><td>字符串拼接，将S1，S2，…..Sn拼接成一个字符串</td></tr><tr><td>LOWER(str)</td><td>将字符串str全部转为小写</td></tr><tr><td>UPPER(str)</td><td>将字符串str全部转为大写</td></tr><tr><td>LPAD(str,n,pad)</td><td>左填充，用字符串pad对str的左边进行填充，达到n个字符串长度</td></tr><tr><td>RPAD(str,n,pad)</td><td>右填充，用字符串pad对str的右边进行填充，达到n个字符串长度</td></tr><tr><td>TRIM(str)</td><td>去掉字符串头部和尾部的空格</td></tr><tr><td>SUBSTRING(str,start,len)</td><td>返回从字符串str从start位置起的len个长度的字符串</td></tr></tbody>
</table></figure>
<h3>2.2 数值函数</h3>
<figure class='table-figure'><table>
<thead>
<tr><th>函数</th><th>功能</th></tr></thead>
<tbody><tr><td>CEIL(x)</td><td>向上取整</td></tr><tr><td>FLOOR(x)</td><td>向下取整</td></tr><tr><td>MOD(x,y)</td><td>返回x/y的模</td></tr><tr><td>RAND()</td><td>返回0~1内的随机数</td></tr><tr><td>ROUND(x,y)</td><td>求参数x的四舍五入的值，保留y位小数</td></tr></tbody>
</table></figure>
<h3>2.3 日期函数</h3>
<figure class='table-figure'><table>
<thead>
<tr><th>函数</th><th>功能</th></tr></thead>
<tbody><tr><td>CURDATE()</td><td>返回当前日期</td></tr><tr><td>CURTIME()</td><td>返回当前时间</td></tr><tr><td>NOW()</td><td>返回当前日期和时间</td></tr><tr><td>YEAR(date)</td><td>获取指定date的年份</td></tr><tr><td>MONTH(date)</td><td>获取指定date的月份</td></tr><tr><td>DAY(date)</td><td>获取指定date的日期</td></tr><tr><td>DATE_ADD(date, INTERVAL expr type)</td><td>返回一个日期/时间值加上一个时间间隔expr后的时间值</td></tr><tr><td>DATEDIFF(date1,date2)</td><td>返回起始时间date1 和 结束时间date2之间的天数</td></tr></tbody>
</table></figure>
<h3>2.4 流程函数</h3>
<figure class='table-figure'><table>
<thead>
<tr><th>函数</th><th>功能</th></tr></thead>
<tbody><tr><td>IF(value ,t, f)</td><td>如果value为true，则返回t，否则返回f</td></tr><tr><td>IFNULL(value1 , value2)</td><td>如果valuel不为空，返回value1，否则返回value2</td></tr><tr><td>CASE WHEN [vall ] THEN [res] ... ELSE[default] END</td><td>如果vall为true，返回res1l，. 否则返回default默认值</td></tr><tr><td>CASE [expr ]  WHEN [val1 ] THEN [res1] ... ELSE[ default ]  END</td><td>如果expr的值等于vall，返回res1，.否则返回default默认值</td></tr></tbody>
</table></figure>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h2>3 约束</h2>
<figure class='table-figure'><table>
<thead>
<tr><th>约束</th><th>描述</th><th>关键字</th></tr></thead>
<tbody><tr><td>非空约束</td><td>限制该字段的数据不能为null</td><td>NOT NULL</td></tr><tr><td>唯一约束</td><td>保证该字段的所有数据都是唯一、不重复的</td><td>UNIQUE</td></tr><tr><td>主键约束</td><td>主键是一行数据的唯一标识，要求非空且唯一</td><td>PRIMARY KEY</td></tr><tr><td>默认约束</td><td>保存数据时，如果未指定该字段的值，则采用默认值</td><td>DEFAULT</td></tr><tr><td>检查约束</td><td>保证字段值满足某一个条件</td><td>CHECK</td></tr><tr><td>外键约束</td><td>用来让两张表的数据之间建立连接，保证数据的一致性和完整性</td><td>FOREIGN KEY</td></tr></tbody>
</table></figure>
<h3>外键约束</h3>
<h4>添加外键</h4>
<pre><code class='language-sql' lang='sql'>CREATE TABLE 表名(
字段名 数据类型,
...
[CONSTRAINT] 外键名称  FOREIGN KEY(外键字段名) REFERENCES 主表(主表列名)
);
</code></pre>
<pre><code>ALTER TABLE 表名 ADD CONSTRAINT 外键名称 FOREIGN KEY(外键字段名）REFERENCES 主表(主表列名);
</code></pre>
<p>注意：添加外键时的指向的主表字段一定要是主键</p>
<p><img src="D:\Typora\save\MySQL\assets\添加外键代码.png"  /></p>
<pre><code class='language-sql' lang='sql'>SELECT * FROM table_1 WHERE ID &lt; 4 AND ID &gt; 1 LIMIT 0 ,2;

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


INSERT INTO SCHOOL VALUES (1,&#39;任远&#39;),(2,&#39;一中&#39;),(3,&#39;二中&#39;),(4,&#39;玉树&#39;);

INSERT INTO STUDENT VALUES (1, &#39;张三&#39;, 1,1),(2,&#39;李四&#39;,2, &#39;2&#39;),
                           (3,&#39;王五&#39;,1,1),(4,&#39;麻子&#39;,1,1),

                           (5,&#39;丁一&#39;, 6,4),(6,&#39;牛二&#39;,5,3);
</code></pre>
<p>&nbsp;</p>
<p><img src="D:\Typora\save\MySQL\assets\添加外键的表1.png" referrerpolicy="no-referrer"></p>
<p><img src="D:\Typora\save\MySQL\assets\添加外键的表2.png" referrerpolicy="no-referrer"></p>
<p>&nbsp;</p>
<h4>删除外键</h4>
<pre><code>ALTER TABLE 表名 DROP FOREIGN KEY 外键名称;
</code></pre>
<p>删除更新行为</p>
<figure class='table-figure'><table>
<thead>
<tr><th>行为</th><th>说明</th></tr></thead>
<tbody><tr><td>NO ACTION</td><td>当在父表中删除/更新对应记录时，首先检查该记录是否有对应外键，如果有则不允许删除/更新。 (与 RESTRICT一致)</td></tr><tr><td>RESTRICT</td><td>当在父表中删除/更新对应记录时，首先检查该记录是否有对应外键，如果有则不允许删除/更新。 (与 NO ACTION 一致)</td></tr><tr><td>CASCADE</td><td>当在父表中删除/更新对应记录时，首先检查该记录是否有对应外键，如果有，则也删除/更新外键在子表中的记录。</td></tr><tr><td>SET NULL</td><td>当在父表中删除对应记录时，首先检查该记录是否有对应外键，如果有则设置子表中该外键值为null（这就要求该外键允许取nulI）。</td></tr><tr><td>SET DEFAULT</td><td>父表有变更时，子表将外键列设置成一个默认的值 (Innodb不支持)</td></tr></tbody>
</table></figure>
<p>&nbsp;</p>
<h2>4  连接查询</h2>
<h3>4.1 连接查询-内连接</h3>
<p><strong>隐式内连接</strong></p>
<pre><code class='language-sql' lang='sql'>SELECT 字段列表 FROM 表1, 表2 WHERE条件 ...;
</code></pre>
<p><strong>显式内连接</strong></p>
<pre><code class='language-sql' lang='sql'>SELECT 字段列表 FROM 表1 [INNER] JOIN 表2 ON 连接条件 ..;
</code></pre>
<p>内连接查询的是两张表交集的部分</p>
<p><img src="D:\Typora\save\MySQL\assets\连接查询.png" referrerpolicy="no-referrer"></p>
<h3>4.2 连接查询-外连接</h3>
<p><strong>左外连接</strong></p>
<pre><code class='language-sql' lang='sql'>SELECT 字段列表 FROM 表A LEFT [OUTER] JOIN 表B ON 条件 ...;
</code></pre>
<p><img src="D:\Typora\save\MySQL\assets\左外连接.png" referrerpolicy="no-referrer"></p>
<p>相当于查询表A(左表)的所有数据，包含表A和表B交集部分的数据</p>
<p>注意最后一行数据，为了体现出与内连接的区别，这里添加了一行数据，因为这名学生schoolid字段为空，使用内连接会无法查询到该学生信息</p>
<p><strong>右外连接</strong></p>
<pre><code class='language-sql' lang='sql'>SELECT 字段列表 FROM 表A RIGHT [OUTER] JOIN 表B ON 条件 ...;
</code></pre>
<p>相当于查询表B(右表)的所有数据，包含表A和表B交集部分的数据</p>
<h3>4.3 连接查询-自连接</h3>
<p>自连接查询语法：</p>
<pre><code class='language-sql' lang='sql'>SELECT 字段列表 FROM 表A 别名A JOIN 表A  别名B ON 条件...
</code></pre>
<p>自连接查询，可以是内连接查询，也可以是外连接查询。</p>
<h3>4.4 联合查询-union，unionall</h3>
<p>对于union查询，就是把多次查询的结果合并起来，形成一个新的查询结果集。</p>
<pre><code class='language-sql' lang='sql'>SELECT 字段列表 FROM 表A...
UNION [ALL]
SELECT 字段列表 FROM 表B...;
</code></pre>
<p>对于联合查询的多张表的列数必须保持一致，字段类型也需要保持一致。</p>
<p>unionall会将全部的数据直接合并在一起，union会对合并之后的数据去重。</p>
<h3>4.5 子查询</h3>
<p>概念：SQL语句中嵌套SELECT语句，称为嵌套查询，又称子查询。</p>
<pre><code class='language-sql' lang='sql'>SELECT * FROM tl WHERE column1 = (SELECT column1 FROM t2);
</code></pre>
<p><strong>子查询外部的语句可以是INSERT/UPDATE/DELETE／SELECT的任何一个。</strong></p>
<p>根据子查询结果不同，分为：</p>
<ul>
<li>标量子查询 (子查询结果为单个值)</li>
<li>列子查询(子查询结果为一列)</li>
<li>行子查询(子查询结果为一行)</li>
<li>表子查询(子查询结果为多行多列)</li>

</ul>
<p>根据子查询位置，分为：WHERE之后、FROM之后、SELECT 之后。</p>
<h4>4.5.1 标量子查询</h4>
<p>子查询返回的结果是单个值（数字、字符串、日期等），最简单的形式，这种子查询成为标量子查询。</p>
<p>常用的操作符：=  &lt;&gt;  &gt;   &gt;=   &lt;  &lt;=</p>
<p>示例：查询来自任远的学生信息（学校信息表和学生信息表见上）</p>
<p>此例可以分两个步骤来做，首先查询学校信息表中任远中学的编号：</p>
<p><img src="D:\Typora\save\MySQL\assets\标量子查询示例1.png" referrerpolicy="no-referrer"></p>
<p>结果返回1，这时再查询学校编号在学生信息表中对应的学生：</p>
<p><img src="D:\Typora\save\MySQL\assets\标量子查询示例2.png" referrerpolicy="no-referrer"></p>
<p>而利用标量子查询可以用一行代码解决这个问题，标量子查询的关键在于把代码看出一个值，如步骤一代码返回值为是学校编号，那就把这行代码看作是学校编号，同理，在后页面的表子查询中，代码返回一张表，那就可以把代码当成一张表在其它代码中使用。</p>
<p>注意：使用时要加括号</p>
<p><img src="D:\Typora\save\MySQL\assets\标量子查询示例3.png" referrerpolicy="no-referrer"></p>
<h4>4.5.2 列子查询</h4>
<p>子查询返回的结果是一列（可以是多行），这种子查询称为列子查询。</p>
<p>常用的操作符：IN、NOTIN、ANY、SOME、ALL</p>
<figure class='table-figure'><table>
<thead>
<tr><th>操作符</th><th>描述</th></tr></thead>
<tbody><tr><td>IN</td><td>在指定的集合范围之内，多选一</td></tr><tr><td>NOT IN</td><td>不在指定的集合范围之内</td></tr><tr><td>ANY</td><td>子查询返回列表中，有任意一个满足即可</td></tr><tr><td>SOME</td><td>与ANY等同，使用SOME的地方都可以使用ANY</td></tr><tr><td>ALL</td><td>子查询返回列表的所有值都必须满足</td></tr></tbody>
</table></figure>
<h4>4.5.3  行子查询</h4>
<p>子查询返回的结果是一行（可以是多列），这种子查询称为行子查询。</p>
<p>常用的操作符：=、&lt;&gt;、IN、NOT IN</p>
<p>补充知识点：</p>
<pre><code class='language-sql' lang='sql'>SELECT * FROM 表A WHERE 字段1 = 值1 AND 字段2 = 值2; 
</code></pre>
<pre><code class='language-sql' lang='sql'>SELECT * FROM 表A WHERE (字段1, 字段2) = (值1, 值2); 
</code></pre>
<p>两种写法等效</p>
<h4>4.5.4 表子查询</h4>
<p>子查询返回的结果是多行多列，这种子查询称为表子查询</p>
<p>常用的操作符：IN</p>
<p>补充知识点：</p>
<pre><code class='language-sql' lang='sql'>SELECT * FROM 表A WHERE (字段1, 字段2) IN (表b); 
</code></pre>
<p>表b中的字段与括号内字段相同，可以查询到表a中满足两字段等于表b中任何一行数据的数据</p>
<p>&nbsp;</p>
<h2>5 事务</h2>
<h3>5.1 事务操作</h3>
<h4>5.1.1 查看/设置事务提交方式</h4>
<pre><code class='language-sql' lang='sql'>SELECT @@autocommit ;
SET @@autocommit = 0;
# 1：自动	0：手动 
</code></pre>
<h4>5.1.2 开启事务</h4>
<pre><code class='language-sql' lang='sql'>START TRANSACTION 或 BEGIN ;
</code></pre>
<h4>5.1.3 提交事务</h4>
<pre><code class='language-sql' lang='sql'>COMMIT ;
</code></pre>
<h4>5.1.4 回滚事务</h4>
<pre><code class='language-sql' lang='sql'>ROLLBACK ;
</code></pre>
<h3>5.2 <font color='red'>事务四大特性</font></h3>
<p><strong>原子性</strong>（<font color='red'>A</font>tomicity）：事务是不可分割的最小操作单元，要么全部成功，要么全部失败。</p>
<p><strong>一致性</strong>（<font color='red'>C</font>onsistency）：事务完成时，必须使所有的数据都保持一致状态。</p>
<p><strong>隔离性</strong>（<font color='red'>I</font>solation）：数据库系统提供的隔离机制，保证事务在不受外部并发操作影响的独立环境下运行。</p>
<p><strong>持久性</strong>（<font color='red'>D</font>urability）：事务一旦提交或回滚，它对数据库中的数据的改变就是永久的。</p>
<h3>5.3 并发事务问题</h3>
<figure class='table-figure'><table>
<thead>
<tr><th>问题</th><th>描述</th></tr></thead>
<tbody><tr><td>脏读</td><td>一个事务读到另外一个事务还没有提交的数据。</td></tr><tr><td>不可重复读</td><td>一个事务先后读取同一条记录，但两次读取的数据不同，称之为不可重复读。</td></tr><tr><td>幻读</td><td>一个事务按照条件查询数据时，没有对应的数据行，但是在插入数据时，又发现这行数据已经存在，好像出现了&quot;幻影&quot;。</td></tr></tbody>
</table></figure>
<h3>5.4 事务隔离级别</h3>
<h4>5.4.1 隔离级别</h4>
<figure class='table-figure'><table>
<thead>
<tr><th>隔离级别</th><th>脏读</th><th>不可重复读</th><th>幻读</th></tr></thead>
<tbody><tr><td>Read uncommitted</td><td>√</td><td>√</td><td>√</td></tr><tr><td>Read committed</td><td>×</td><td>√</td><td>√</td></tr><tr><td>Repeatable Read(默认)</td><td>×</td><td>×</td><td>√</td></tr><tr><td>Serializable</td><td>×</td><td>×</td><td>×</td></tr></tbody>
</table></figure>
<h4>5.4.2 查看事务隔离级别</h4>
<pre><code class='language-sql' lang='sql'>SELECT @@TRANSACTION_ISOLATION;
</code></pre>
<h4>5.4.2 设置事务隔离级别</h4>
<pre><code class='language-sql' lang='sql'>SET [SESSION | GLOBAL] TRANSACTION ISOLATION LEVEL { READ UNCOMMITTED | READ COMMITTED | REPEATABLE READ | SERIALIZABLE } 
</code></pre>
<p>注意：事务隔离级别越高。数据安全性越好，但同时性能也会越差</p>
<h1>MySQL从入门到入土——进阶篇</h1>
<h2>MySQL体系结构</h2>
<p><img src="D:\Typora\save\MySQL\assets\MySQL体系结构图.png" referrerpolicy="no-referrer"></p>
<p><strong>连接层</strong>
最上层是一些客户端和链接服务，主要完成一些类似于连接处理、授权认证、及相关的安全方案。服务器也会为安全接入的每个客户
端验证它所具有的操作权限。
<strong>服务层</strong>
第二层架构主要完成大多数的核心服务功能，如SQL接口，并完成缓存的查询，SQL的分析和优化，部分内置函数的执行。所有跨存
储引擎的功能也在这一层实现，如过程、函数等。
<strong>引擎层</strong>
存储引擎真正的负责了MySQL中数据的存储和提取，服务器通过API和存储引擎进行通信。不同的存储引擎具有不同的功能，这样我
们可以根据自己的需要，来选取合适的存储引擎。
<strong>存储层</strong>
主要是将数据存储在文件系统之上，并完成与存储引擎的交互</p>
<p>&nbsp;</p>
<h2>存储引擎</h2>
<h3>存储引擎简介</h3>
<p>存储引擎就是存储数据、建立索引、更新/查询数据等技术的实现方式。存储引擎是基于表的，而不是基于库的，所以存储引擎也可被
称为表类型。</p>
<p>&nbsp;</p>
<p>在创建表时，指定存储引擎</p>
<pre><code>CREATE TABLE 表名(
字段1字段1类型型[ COMMENT 字段1注释],
...

字段n 字段n类型[COMMENT 字段n注释]
)ENGINE=INNODB [COMMENT 表注释];
</code></pre>
<p>查看当前数据库支持的存储引擎</p>
<pre><code>SHOW ENGINES ;
</code></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h4>InnoDB</h4>
<p>介绍
InnoDB是一种兼顾高可靠性和高性能的通用存储引擎，在 MySQL 5.5 之后，InnoDB是默认的 MySQL 存储引擎。
特点
DML操作遵循ACID模型，支持事务;
行级锁，提高并发访问性能;
支持外键 FOREIGN KEY约束，保证数据的完整性和正确性;
文件
xxx.ibd：xxx代表的是表名，innoDB引擎的每张表都会对应这样一个表空间文件，存储该表的表结构（frm、sdi）、数据和索引。
参数： innodb_file_per_table </p>
<p>&nbsp;</p>
<h4>MylSAM</h4>
<p>介绍
MyISAM是MySQL早期的默认存储引擎。
特点
不支持事务，不支持外键
支持表锁，不支持行锁
访问速度快
文件
xxx.sdi：存储表结构信息
xxx.MYD:存储数据
xxx.MYI:存储索引I</p>
<p>&nbsp;</p>
<h4>Memory</h4>
<p>介绍
Memory引擎的表数据时存储在内存中的，由于受到硬件问题、或断电问题的影响，只能将这些表作为临时表或缓存使用。
特点
内存存放
hash索引 (默认）
文件
xxx.sdi：存储表结构信息</p>
<p>&nbsp;</p>
<h3>存储引擎特点</h3>
<figure class='table-figure'><table>
<thead>
<tr><th>特点</th><th>InnoDB</th><th>MyISAM</th><th>Memory</th></tr></thead>
<tbody><tr><td>存储限制</td><td>64TB</td><td>有</td><td>有</td></tr><tr><td>事务安全</td><td>支持</td><td>-</td><td>-</td></tr><tr><td>锁机制</td><td>行锁</td><td>表锁</td><td>表锁</td></tr><tr><td>B+tree索引</td><td>支持</td><td>支持</td><td>支持</td></tr><tr><td>Hash索引</td><td>-</td><td>-</td><td>支持</td></tr><tr><td>全文索引</td><td>支持(5.6版本之后)</td><td>支持</td><td>-</td></tr><tr><td>空间使用</td><td>高</td><td>低</td><td>N/A</td></tr><tr><td>内存使用</td><td>高</td><td>低</td><td>中等</td></tr><tr><td>批量插入速度</td><td>低</td><td>高</td><td>高</td></tr><tr><td>支持外键</td><td>支持</td><td>-</td><td>-</td></tr></tbody>
</table></figure>
<h3>存储引擎选择</h3>
<p>在选择存储引擎时，应该根据应用系统的特点选择合适的存储引擎。对于复杂的应用系统，还可以根据实际情况选择多种存储引擎进行组
合。
<strong>InnoDB</strong>：是Mysql的默认存储引擎，支持事务、外键。如果应用对事务的完整性有比较高的要求，在并发条件下要求数据的一致
性，数据操作除了插入和查询之外，还包含很多的更新、删除操作，那么InnoDB存储引擎是比较合适的选择。</p>
<p><strong>MyISAM</strong>：如果应用是以读操作和插入操作为主，只有很少的更新和删除操作，并且对事务的完整性、并发性要求不是很高，那
么选择这个存储引擎是非常合适的。</p>
<p><strong>MEMORY</strong>：将所有数据保存在内存中，访问速度快，通常用于临时表及缓存。MEMORY的缺陷就是对表的大小有限制，太大的表
无法缓存在内存中，而且无法保障数据的安全性。</p>
<p>&nbsp;</p>
<h2>索引</h2>
