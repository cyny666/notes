在我们导入python脚本时在目录下会生成一个相应的pyc文件，是pythoncodeobj的持久化储存形式，加速下一次的装载

### 文件结构

pyc文件由三大部分组成

* 最开始4个字节是一个Maigc int，表示此pyc的版本信息
* 接下来四个字节还是个int，是pyc产生的时间
* 序列化的PyCodeObject

