# pathping 
## chatgpt 
pathping是一个Windows命令行实用程序，用于评估IP数据包在网络上传输时的延迟，丢失和带宽问题。

pathping命令与tracert和ping命令类似，但是pathping可以在时间内执行跟踪路由和测量异步延迟，同时为每个路由器节点提供丢包统计信息。

使用pathping命令时，它会生成一份详细的路由跟踪报告，其中包括每个路由器的IP地址，计算的平均往返时间，以及在评估到每个节点的并发连接中丢失的数据包的数量。

pathping命令可以用于识别网络上的瓶颈和丢包问题，并帮助管理员更好地了解网络的拓扑结构。对于用户而言，pathping可以用于诊断网站或互联网连接的速度慢或不可用的问题。 

## tldr 
 
> 一种结合了`ping`和`tracert`功能的跟踪路由工具。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/pathping>.

- Ping 并追踪主机的路由：

`pathping {{主机名}}`

- 不要对主机名执行 IP 地址的反向查找：

`pathping {{主机名}} -n`

- 指定要搜索目标的最大跃点数（默认值为 30）：

`pathping {{主机名}} -h {{最大跃点数}}`

- 指定 ping 之间等待的毫秒数（默认值为 240）：

`pathping {{主机名}} -p {{时间}}`

- 指定每跳的查询数（默认值为 100）：

`pathping {{主机名}} -q {{查询语句}}`

- 强制使用 IPV4：

`pathping {{主机名}} -4`

- 强制使用 IPV6：

`pathping {{主机名}} -6`

- 显示详细的使用帮助：

`pathping /?`
