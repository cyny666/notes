SQL对大小写不敏感、SELECT与select是相同的

一些重要的SQL命令：

* SELECT-从数据库中提取数据
* UPDATE-更新数据库中的数据
* DELETE-从数据库中删除数据
* INSERT INFO-向数据库中插入新数据
* CREATE DATABASE：创建新数据库
* ALTER DATABASE-修改数据库
* CREATE：创建新表
* ALTER TABLE：变更数据库表
* DROP TBALE：删除表
* CREATE INDEX：创建索引
* DROP INDEX：删除索引

SQL ORDER BY 关键字

ASC：表示按升序排序 DESC：表示按降序排序

sql中的通配符：

%：代替0个或多个字符 -：代替一个字符 

[charlist]:字符列中的任何单一字符，mysql中使用regexp或者not regexp运算符来匹配正则表达式

约束：

* NOT NULL-指示某列不能存储NULL值
* UNIQUE-保证某列的每行必须有唯一的值
* PRIMARY KEY - NOT NULL和UNIQUE的结合，确保某列（或两个列多个列的结合）有唯一标识，有助于更容易更快速地找到表中的一个特定的记录。
* FOREIGN KEY- 保证一个表中的数据匹配另一个表中的值的参照完整性。
* CHECK-保证列中的值符合指定的条件
* DEFAULT-规定没有给列赋值的默认值

sql函数：

* AVG()-返回平均值
* COUNT()-返回行数
* FIRST()-返回第一个记录的值
* LAST()-返回最后一个记录的值
* MAX()-返回最大值
* MIN()-返回最小值
* SUM()-返回总和
* UCASE()-将某个字段转换为大写
* MID()-从某个文本字段提取字符，mysql中使用
* SubString(字段，1，end)-从某个文本字段提取字符
* LEN()-返回某个文本字段的长度
* ROUND()-对某个数值
* NOW()-返回当前的系统日期和时间
* FORMAT()-格式化某个字段的显示方式



