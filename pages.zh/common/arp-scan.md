# arp-scan 
## chatgpt 
arp-scan是一个命令行实用程序，可扫描局域网中的IP地址和MAC地址。它使用ARP协议（地址解析协议）来查询主机和其它网络上的设备，并返回其MAC地址和IP地址。

命令格式：

arp-scan [选项] [目标IP地址]

选项：

- -I interface: 指定网络接口，默认使用eth0
- -l: 列出扫描到的所有IP地址和MAC地址
- -g: 扫描整个局域网，不需要指定目标IP地址
- -r: 随机扫描局域网，使用该选项可以防止被防火墙阻拦
- -t: 设置扫描超时时间（默认为1秒）
- -s: 指定源IP地址
- -n: 不进行反向DNS查询

例如，要扫描192.168.1.0/24网段并列出结果，可以使用以下命令：

sudo arp-scan -l -I eth0 192.168.1.0/24

这将扫描192.168.1.0到192.168.1.255之间所有主机并显示它们的IP地址和MAC地址。需要以root用户运行此命令。 

## tldr 
 
> 发送 ARP 数据包到特定主机（指定 IP 地址或主机名），来扫描本地网络。
> 更多信息：<https://github.com/royhills/arp-scan>.

- 扫描当前本地网络：

`arp-scan --localnet`

- 扫描带有自定义位掩码的 IP 网络：

`arp-scan {{192.168.1.1}}/{{24}}`

- 扫描自定义范围内的 IP 网络：

`arp-scan {{127.0.0.0}}-{{127.0.0.31}}`

- 扫描带有自定义子网掩码的 IP 网络：

`arp-scan {{10.0.0.0}}:{{255.255.255.0}}`
