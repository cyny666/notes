### 文件结构

一个GIF文件的结构可分为

* 文件头（File Header）
  * GIF文件署名（Signature）
  * 版本号（Version）
* GIF数据流（GIF Data Stream）
  * 控制标识符
  * 图象块（Image Block）
  * 其他的一些扩展块
* 文件终结器（Trailer）

### 文件头

GIF署名（Signature）和版本号（Version）。GIF署名用来确认一个文件是否是GIF格式的文件，这一部分由三个字符组成：GIF；文件版本号也是由三个字节组成，可以为87a或89a

### 逻辑屏幕标识符

Logical Screen Descriptor紧跟在header后面。这个块告诉decoder图片需要占用的空间。它的大小固定为7个字节，以canvas width（画布宽度）和canvas height（画布高度）开始

### 全局颜色列表

GIF格式可以拥有global color table，或用于针对每个字图片集，提供local color table。每个color table由一个RGB（就像通常我们见到的（255,0,0）红色那种）列表组成。

### 图像标识符

一个GIF文件一般包含多个图片。之前的图片渲染模式一般是将多个图片绘制到一个大的（virtual canvas）虚拟画布上，而现在一般将这些图片集用于实现动画

每个image都以一个image descriptor block（图像描述块）作为开头，这个块固定为10字节。

### 图像数据

终于到了图片数据实际存储的地方。Image Data是由一系列的输出编码（output codes）构成，它们告诉decoder（解码器）需要绘制在画布上的每个颜色信息。这些编码以字节码的形式组织在这个块中。

### 文件终结器

该块为一个单字段块，用来指示该数据流的结束。取固定值0x3b

### 空间轴

由于GIF的动态特性，由一帧帧的图片构成，所以每一帧的图片，多帧图片间的结合，都成了隐藏信息的一种载体。

对于需要分离的GIF文件，可以使用convert命令将其每一帧分割开来

