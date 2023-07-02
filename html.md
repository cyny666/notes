1.文档后缀名

.html .htm

2.简介

* \<!DOCTYPE html>声明为HTML5文档
* \<html>元素是HTML页面的根元素
* \<head>元素包括了文档的元(meta)数据，如\<meta charset="utf-8">定义网页编码格式为uft-8
* \<title>元素描述了文档的标题
* \<body>元素包含了可见的页面内容
* \<h1>元素定义了一个大标题
* \<P>元素定义一个段落

浏览器上使用F12按键开启调试模式，就可以看到组成标签

\<标签>内容\</标签>

HTML标题是通过<h1>-<h6>定义的

HTML段落是通过标签<p>来定义的

HTML链接是通过标签<a>来定义的（在href属性中指定链接的地址）

HTML图像是通过标签<img>来定义的（图像的名称和尺寸是以属性的形式提供的)

当属性值本身就含有双引号，那么必须使用单引号

HTML的大多数属性：

* class:为html元素定义一个或多个类名(类名从样式文件引入)
* id:定义元素的唯一id
* style:规定元素的行内样式
* title:描述了元素的额外信息

\<hr>标签在HTMl页面中创建水平线

\<!-- 这是一个注释 -->

可以使用\<br>折行

* <b>:定义粗体文本
* <em>:定义着重文字
* <i>:定义斜体文字
* <small>:定义小号字
* <strong>:定义加重语气
* <sub>:定义下标字
* <sup>:定义上标字
* <ins>：定义插入字
* <del>:定义删除字
* <code>:定义计算机代码
* <kbd>:定义键盘码
* <samp>:定义计算机代码样本
* <var>:定义变量
* \<pre>：定义预格式文本
* <abbr>:定义缩写
* \<address>:定义缩写
* \<bdo>:定义文字方向
* \<blockquote>:定义长的引用
* \<q>:定义短的引用
* \<cite>:定义引用、引证
* \<dfn>:定义一个定义项目

### html链接

target属性定义被链接的文档在何处显示

id属性可用于创建一个HTML文档书签 可用"#tips"来访问id=tips的部分

### html头部

\<title>元素：

* 定义了浏览器工具栏的标题
* 当网页添加到收藏夹
* 显示在搜索引擎结果页面的标题

\<base>标签描述了基本的链接地址/链接目标，改标签作为HTML文档中所有的链接标签的默认链接

\<link>标签定义了文档与外部资源之间的关系(link标签通常用于链接到样式表)

\<style>标签定义了HTML文档的样式文件引用地址(style元素中也可以直接添加样式来渲染HTML文档)

\<meta>标签提供了元数据，通常用于指定网页的描述，关键词，文件的最后修改时间，作者，和其他元数据

\<script>: 用于加载脚本文件

### html样式-css

背景颜色(background-color)、font-family(字体)、color(颜色)、font-size(字体大小)、text-align(文字对齐)

### html图像

\<img src="url" alt="some_text"> src是指source，是图像的URL地址

alt属性用来为图像定义一串预备的可替换的文本(主要告诉读者他们失去的信息)

height、weight用于设置图像的高度与宽度

### html表格

表格由<table>标签来定义。每个标签均有若干行（由<tr>标签定义），每行被分割成若干单元格(由<td>标签定义)

### html列表

无序列表用<ul>标签

自定义列表以<dl>标签开始。每个自定义列表项以<dt>开始。每个自定义列表项的定义以<dd>开始

div元素是用于分组HTML元素的块级元素

### html表单和输入

文本域通过<input type="text">

密码字段通过标签<input type="password">来定义

单选按钮：<input type="radio">

复选框：<input type="checkbox">

提交按钮：<input type="submit">

### html框架

\<iframe src="URL"></iframe>

可以用height和width属性来定义iframe的高度与宽度

frameborder属性用于定义iframe表示是否显示边框

### html脚本

\<script>标签用于定义客户端脚本，比如javascript.

\<noscript>标签：只有在浏览器不支持脚本或者禁用脚本时，才会显示<noscript>元素中的内容

scheme：//host.domain:port/path/filename

scheme:定义因特网服务的类型，常见的类型是http

host：定义域主机（http默认是www）

domain：定义因特网域名

：port：定义主机上的端口号

path：定义服务器上的路径

filename：定义文档/资源的名称

