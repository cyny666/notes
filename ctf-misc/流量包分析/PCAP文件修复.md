### PCAP文件结构

一般来说，对于PCAP文件格式考察较少，且通常都能借助于现成的工具如pcapfix直接修复，这里大致介绍下几个常见的块。

* Tools
  * PcapFix Online
  * PcapFix

目前所定义的常见块类型有

* Section Header Block:it defines the most important characteristics of the capture file
* Interface Description Block:it defines the most important characteristics of the interface used for captruing traffic
* Packet Block:it contains a single captured packet,or a portion of it,with only a minimal set of information about it
* Name Resolution Block:it defines the mapping from numeric addresses present in the packet dump and the canonical name counterpart
* Capture Statistics Block: it defines how to store some statistical data(e.g. packet dropped,etc)which can be useful to understand the conditions in which the capture has been made.

### 常见块

### Section Header Block(文件头)

必须存在，意味着文件的开始

### Interface Description Block(接口描述)

必须存在，描述接口特性

### Packet Block(数据块)

