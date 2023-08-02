直接写入HTML输出流 document.write

对事件的反应 ：alert函数

改变HTML内容：document.getElementById("demo")

Javascript脚本代码必须位于<script>与</script>之间

JavaScript脚本代码可被放置在HTML页面的<body>和<head>部分中

外局脚本不能包含<script>标签

JavaScript可以通过不同的方式来输出数据:

* 使用window.alert()弹出警告框
* 使用document.write()方法将内容写到HTML文档中
* 使用innerHTML写入到HTML元素
* 使用console.log()写入到浏览器的控制台

定义函数 function myFunction(a,b) {return a*b;}

JavaScript使用关键字var来定义变量，使用等号来为变量赋值

JavaScript拥有动态类型。变量的数据类型可以使用typeof操作符来查看

Undefined这个值表示变量不含有值、可以通过将变量的值设置为null来清空变量

创建对象： 

```javascript
var person = {firstname:"John", lastname:"Doe", age:50,eyecolor:"blue"};
```

创建对象方法:

methodName:function(){}

常见的html事件

| 事件        | 描述                               |
| ----------- | ---------------------------------- |
| onchange    | HTML元素改变                       |
| onclick     | 用户点击HTML元素                   |
| onmouseover | 鼠标指针移动到指定的元素上时发生   |
| onmouseout  | 用户从一个HTML元素上移开鼠标时发生 |
| onkeydown   | 用户按下键盘按键                   |
| onload      | 浏览器已完成页面的加载             |

JavaScript严格模式(strict mode)即在严格的条件下运行

let声明的变量只在let命令所在的代码块内有效

const声明一个只读的常量，一旦声明，常量的值就不能改变

JavaScript：void(0)中最关键的是void关键字，void是JavaScript中非常重要的关键字，该操作符指定要计算一个表达式但是不返回值

addEventListener()方法用于向指定元素添加事件句柄，在捕获中，外部元素的事件会先被触发，然后才会触发内部元素的事件

我们可以用replaceChild()方法来替换HTML DOM中的元素



