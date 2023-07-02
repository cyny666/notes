php的EOF结束标识必须顶格独占一行

php支持一下几种数据类型：

* string(字符型)
* Integer(整形)
* Float(浮点型)
* Boolean(布尔型)
* Array(数组)
* Object(对象)
* NULL(空值)
* Resource(资源)

php中var_dump()函数返回变量的数据类型和值：

php中必须用class声明对象

常见资源类型有打开文件、数据库连接、图形画布区域

get_resource_type(resource $handle):string

松散比较：使用两个等号：==，只比较值，不比较类型

严格比较：用三个等号：===，除了比较值，也比较类型

常量在整个脚本中都可以使用：

设置常量，使用define()函数：bool define (string $name, mixed $value [, bool $case_insenstive = false]) 

name:必选参数，常量名称

value:必选参数，常量的值

php中只有一个字符串运算符，并置运算符(.)用于把两个字符串值连接起来

strpos()函数用于在字符串内查找一个字符或一段指定的文本

intdiv()该函数的返回值为第一个参数除于第二个参数的值并取整(向下取整)

不等于：x<>y

三元运算符：

(expr1) ? (expr2) : (expr3)

对expr1求值为true时的值为expr2,在expr1的值为FALSE的值为expr3

组合比较符：$c = $a <=> $b;

如果$a>$b,则$c的值为1

如果$a==$b,则$c的值为0

如果$a<$b,则$c的值为-1

php超级全局变量列表：

* $GLOBALS:包含了全部变量的全局组合数组
* $_SERVER:包含了诸如头信息、路径、以及脚本位置等等信息的数组
* $_REQUEST:用于收集HTML表单提交的数据
* $_POST:用于广泛收集表单数据
* $_GET:收集URL中发送的数据

php魔术常量：

* \_LINE_:文件中的当前行号
* \_FILE_:文件的完整路径和文件名
* \_DIR_:文件所在的目录
* \_FUNCTION_:函数名称
* \_CLASS_:类的名称
* \_TRAIT_:Trait的名字
* \_METHOD_:返回该方法被定义时的名字
* \_NAMESPACE_:当前命名空间的名称

类使用class关键字后加上类声明

类的变量使用var来声明

php中允许定义一个方法作为构造函数

void __construct

析构函数： void __destruct

使用关键字extends来继承一个类

访问控制：public , protected, private

php中的$\_GET和$\_POST变量用于检索表单中的信息，比如用户输入

&\_SERVER["PHP_SELF"]是超级全局变量，返回当前正在执行脚本的文件名

htmlspecialchars()函数把一些预定义的字符转换为HTML实体

### 任何javascript代码可以添加在<script>标签中

php中，预定义的$\_GET变量用于收集来自method="get"的表单中的值

php中，预定义的$_POST变量用于收集来自method="post"

php中，预定义的$\_REQUEST变量包含了$\_GET、$\_POST、$\_COOKIE的内容

二维数组 ： 

```php
array(
	array(elements...),
	array(elements...))
   
```

php 的date()函数用于格式化时间/日期

fopen()函数用于在php中打开文件

fclose()函数用于关闭打开的文件

feof()函数检测是否已到达文件末尾

fgets()函数用于从文件中逐行读取文件

cookie是一种服务器留在用户计算机上的小文件。isset()函数来确认是否已设置了cookie

php session变量用于存储用户关于用户会话的信息，或者更改用户会话的设置

Session的工作机制是：为每个访客创建一个唯一的id(UID)，并基于这个UID来存储变量

session_start()函数必须位于<html>标签之前

存储和取回session变量的正确方法是使用PHP$_SESSION变量

如果您希望删除某些session数据，可以使用unset()或session_destroy()函数

mail(to,subject,message,headers,parameters)

php过滤器来对输入进行验证：

FILTER_SANITIZE_EMAIL过滤器从字符串中删除电子邮件中的非法字符

FILTER_VALIDATE_EMAIL过滤器验证电子邮箱地址的值

在php中，默认的错误处理很简单。一条错误信息会被发送到浏览器，这条消息带有文件名、行号以及描述错误的消息

异常用于在指定的错误发生时改变脚本的正常流程

filter_var()-通过一个指定的过滤器来过滤单一的变量

filter_var_array()-通过相同的或不同的过滤器来过滤多个变量

filter_input-获取一个输入变量，并对它进行过滤

filter_input_array-获取多个输入变量，并通过相同的或不同的过滤器对它们进行过滤

两种过滤器：

Validating过滤器：

* 用于验证用户输入
* 严格的格式规则(比如URL或E-Mail验证)
* 如果成功则返回预期的类型，如果失败则返回FALSE

Sanitizing过滤器：

* 用于允许或禁止字符串中指定的字符
* 无数据格式规则
* 始终返回字符串

json_encode 对变量进行JSON编码

json_decode对JSON格式的字符串进行解码，转换为PHP变量

json_last_error返回最后发生的错误



