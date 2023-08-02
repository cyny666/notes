css规则由两个主要的部分构成：选择器（你需要改变样式的html元素），以及一条或者多条声明（每条声明由一个属性和一个值组成）

css中id选择器以"#"来定义

插入样式表的方法有三种：外部样式表、内部样式表、内联样式

优先级如下：

内联样式>内部样式>外部样式>浏览器默认样式

font-family属性设置文本的字体系列

font-size属性设置文本的大小

css的四个链接状态：

* link：正常，未访问过的链接
* visited：用户已访问过的链接
* hover：用户鼠标放在连接上时
* active：链接被点击的那一刻

text-decoration属性主要用于删除链接中的下划线

css盒子模型中的部分说明：

* Margin(外边距)：清除边框外的区域，外边距是透明的
* Border(边框)：围绕在内边距和内容外的边框
* Padding(内边距)：清除内容周围的区域，内边距是透明的
* Content(内容)：盒子的内容，显示文本和图像

嵌套选择器

* p{}:为所有p元素指定一个样式
* .marked{}: 为所有class="marked"元素指定一个样式
* .marked p{ }:为所有class="marked"元素内的p元素指定一个样式
* p.marked{}:为所有class="marked"的p元素指定一个样式

visibility:hidden:该元素虽然隐藏了，但仍然会影响布局

visibility:none:隐藏了布局也隐藏

position属性的五个值：static, relative, fixed, absolute, sticky

css overflow属性用于控制内容溢出元素框时显示的方式

css 元素居中对齐：margin:auto; 文本居中对齐：text-align:center

css中的四种组合方式：

* 后代选择器(以空格 分隔)
* 子元素选择器(以大于>号分隔)
* 相邻兄弟选择器(以加号+分隔)
* 普通兄弟选择器(以波浪号~分隔)

css伪类是用来添加一些选择器的特殊效果

css 中属性的透明度是opacity

css网页布局分为以下几个部分：头部区域、菜单导航区域、内容区域、底部区域

css中的！important规则用于增加样式的权重



