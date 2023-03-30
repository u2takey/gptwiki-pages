# gping6 
## chatgpt 
gping6是一个用于IPv6网络的简单ping工具。 它可以用于测试IPv6主机的可达性和延迟。gping6的用法和ping命令类似，可以指定要ping的主机地址，还可以设置ping的次数和间隔时间。 可以使用gping6命令来诊断IPv6网络中的问题或测试IPv6网络的性能。 以下是gping6命令的常见选项：

- -c：指定要发送的ICMP echo消息数目
- -i：指定ping消息的间隔时间（以秒为单位）
- -s：指定要发送的数据包大小
- -t：在三角形输出模式下运行gping6
- -T：设置不使用IP ID字段来测试
- -u：打印收到的ICMP echo回复消息的时间戳
- -v：显示gping6的版本信息
- -h：显示gping6的帮助信息

例如，在IPv6网络上ping一个主机，可以在终端中运行以下命令：gping6 fe80::1 -c 5，这将发送5个ICMP echo消息到地址fe80::1，并显示响应时间。 

## tldr 
 
> 这是 `-p linux ping6` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux ping6`
