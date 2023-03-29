# btm 
## chatgpt 
btm是BitTorrent元数据文件的扩展名，它是一种元数据文件，用于描述BitTorrent文件的内容和结构。在BitTorrent协议中，客户端使用元数据文件来确定如何下载文件，并在下载过程中对其进行验证。

更具体地说，btm文件是一个包含元数据的文本文件，其中包含有关文件名称、大小、分块、散列、注释和创建者的信息。当客户端打开btm文件时，它将使用其中的信息来创建追踪器请求，获取Peers的列表，并开始下载文件的分块。

因此，btm文件是通过BitTorrent协议下载和共享文件时使用的一个重要文件类型，它通常是通过磁力链接或.torrent扩展名的种子文件来获取的。使用适当的BitTorrent客户端，用户可以通过btm文件下载各种内容，包括音乐、电影、电子书、软件等等。 

## tldr 
 
> 命令行`top`的替代品。
> 比 `top` 更轻便，支持跨平台、图表更丰富。
> 更多信息：<https://github.com/ClementTsang/bottom>.

- 展示默认布局（cpu, 内存，温度，磁盘，网络和 进程）：

`btm`

- 开启基础模式，关闭图表和高亮（接近于 `top`）：

`btm --basic`

- 将图表中的小点换成大点：

`btm --dot_marker`

- 展示电池充电和健康状态：

`btm --battery`

- 设置图表刷新间隔和留存数据的时长：

`btm --rate 250 --default_time_value 30000`
