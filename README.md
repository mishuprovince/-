# -
从头开始学

第10集:早起的编程方式

1801年，约瑟夫。玛丽。雅卡尔发霉了可编程纺织机。
1890年美国人口普查，用穿孔纸卡，汇总数据。
1940年，IBM 402核算机，负责算盈亏总额。
1946年，世界第一台通用电子计算机，ENIAC，用大量拆下板，程序在纸上设计好后，给ENIAC连线，，将近三周时间，很繁琐。
1950年代，存储程序计算机出现，用内存储存程序，方便cpu读取，程序和数据都存在“冯诺依曼结构”。命名自 约翰。冯。诺依曼
冯诺依曼计算机的标志是，一个处理器+数据寄存器+指令寄存器+指令地址寄存器+内存，由曼彻斯特大学于1948年建造，绰号“宝宝👶”
1980年代，几乎所有计算机都有穿孔打卡器读取数据，还有插线板。

第11集：编程语言的发展史

第一条指令在内存地址0：0010 1110（前4位是操作码，后四位是内存地址） 意思是读取内存地址14，放入LOAD_A代表的(0010指向的寄存器)。

早起用机器码写程序。pseudo-code(伪代码)对应机器码。

助记符：用指令代替0和1的机器码。通过程序将文字转换成二进制指令，这样cup可识别文字指令。

汇编器读取“汇编语言”写的程序转换成机器码，汇编器能自动分析跳转地址。汇编器不用固定的跳转地址，可以插入可跳转的标签，当程序被传入汇编器，汇编器会自己搞定跳转地址。
编译器:将高级语言转换成低级语言。

第12集编程原理-语句和函数

编程语言让程序员专心解决问题，不用管硬件细节。

第13集算法入门

归并排序：
最短路径：

第14集数据结构
数组
表
队列
栈
树
图

第15课 阿兰图灵

图灵机：
图灵完备：
图灵测试：机器能让人类相信他是人类

第16课软件工程

面向对象编程
版本管理
集成开发环境

第17课 集成开发环境

第18课 操作系统
操作系统是程序与机器之间的媒介。
动态内存分配

第20课文件与文件系统
文件在系统里是碎片化储存的，一个文件会占用一个或多个块。在文件目录文件中会显示每个文件占用那些块，同时会储存源数据（文件名，创建时间，修改时间，权限等）
文件的删除只是删除目录里的记录，数据还是存在块中，当下次有文件需要占用这个块，数据才会被替换。
文件的移动，只是
文件的删除只是删除目录里的记录，数据还是存在块中，当下次有文件需要占用这个块，数据才会被覆盖。
文件的移动是将文件信息从一个目录转移到另一个目录。

第21课 压缩
无损压缩：没有丢失信息
游程编码：减少重复信息
dftba：用字典储存代码和数据的关系，霍夫曼树。
有损压缩：音频MP3：用不同精度编码不同频段，人对于低音感知不强，只能感到震动。wav和flac是无损。
图像jpeg：将图片分解成8*8像素块，然后删除大量高频率像素块。
视频mpeg-4：只存帧与帧之间变化的部分。

第22课 命令行界面
1970年之前，用打字机与机器对话，后来屏幕普及，用屏幕显示计算机反馈的信息，而且便于修改输入错误。
命令行游戏：Zork
现在多用于访问远程服务器




第22课命令行界面
第25课个人计算机革命
解释器和编译器的区别：编译器是提前转换，解释器运行时转换

第26课图形用户界面
1968年恩格尔巴特，在秋季计算机联合会议展示了他的系统，这次演示被视为如今所有演示的祖先。包括，位图图像，文字处理，视屏会议，实时协作编辑文件。商业上失败了。
施乐之星上首次出现“复制，粘贴”，这台计算机上市前，乔布斯参观了实验室对



第28课：计算机网络
计算机近距离构成的小型网络叫局域网（LAN），以太网需要每台计算机有唯一的媒体访问控制地址，即MAC地址。发送数据时，将接收方的MAc地址作为数据的前缀，发送到网络中。
多台计算机共享一个传输媒介，这种方法叫“载波侦听多路访问”，即CSMA。
载体传输速度叫带宽。
载体和其中的设备总称为冲突域。利用交换机将大的冲突域分割成小的冲突域，交换机记录那些MAC地址在那个冲突域里。
路由：在大型网络中，一个地点到另一个地点有多条路径。
专线：这条线路无需共享，自己能随意使用。一般军队，银行和一些机构在使用。
报文交换：可以使用不同的路由传递，使通信更可靠更能容错。
跳数：信息沿着路由的跳转次数。
跳数限制：跳数会记录在信息中心，传输时会更新跳数，检测到某条信息的跳数过高，就知道了路由出现了问题。
数据包：将大报文分成很多小块。数据包中包含目标地址，报文具体格式由互联网协议定义，简称IP。传输大报文的时候会阻塞宽带，之后有小报文传输也需等之前的传输完成，造成宽带阻塞。
TCP/IP:解决数据包乱序问题。同一报文的不同数据包，会经过不同路线到达顺序可能不同。

第29课 互联网 
广域网：WAN
互联网提供商：ISP。互联网提供商通过路由器的WAN口提供网络。
请求YouTube是视频时，将请求数据包传输到互联网主干，主干再到达YouTube的服务器。traceroute查看跳数
UDP：简单快捷。根据端口号将数据包送到目标程序，UDP头部有校验和用于检查数据是否正确。然而UDP不提供数据重发和数据修复机制，接收方得知数据损坏后将数据包丢掉，发送方不知道数据是否传输成功。ip负责将数据包送到正确的计算机，UDP将数据包送到正确的程序。
TCP:可靠。tcp头部也有端口号和校验和，数据包有序号，会同时发送多个包。根据确认码的成功率和来回时间判断网络堵塞程度，调整同时发包数量。
三次握手：sender发送数据包到receiver，receriver接受到数据包后，返回ack1（确认码）。没有收到确认码，会重发。

域名系统：DNS，浏览器输入网址后去DNS服务器查找对应的IP，如果存在会返回IP到浏览器。DNS是树状结构，顶级域名TLS（.com.gov.net.org等），二级域名（google.com），三级域名（image.google.com）。
开放式系统通信参考模型（OSI）
数据链路层操作物理层：MAC，碰撞检测，指数退避等底层协议。
网络层：负责各种报文交换和路由。
传输层：UDP和tcp负责计算机间点对点传输。检测和修复错误。
会话层：使用udp和tcp创建连接，传递信息和关闭连接
表示层：
应用层：

第30课 万维网
万维网的基本单位是单个页面。
统一资源定位器：URL，
超文本传输协议：HTTP，
