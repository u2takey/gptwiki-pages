# ipconfig 
## chatgpt 
ipconfig是Windows操作系统中的一个命令行实用程序，用于获取当前活动连接的网络接口配置信息，包括IP地址、子网掩码、默认网关、DNS等信息。这个工具可以通过命令提示符窗口运行。

ipconfig命令的一些常见选项包括：

1. /all – 显示所有网络接口的详细配置信息。
2. /renew – 重启当前网络接口的IP地址获取。
3. /release – 释放当前网络接口的IP地址。
4. /flushdns – 清除DNS缓存。
5. /displaydns – 显示系统的DNS缓存内容。
6. /registerdns – 将系统的DNS名称与IP地址进行注册。
7. /showclassid – 显示网络适配器指定的类标识符。
8. /setclassid – 将网络适配器与指定的类标识符关联。

通常情况下，使用ipconfig命令可以帮助你快速诊断网络连接问题以及查看网络接口的配置信息。 

## tldr 
 
> 显示和管理 Windows 的网络配置。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/ipconfig>.

- 显示网络适配器列表：

`ipconfig`

- 显示网络适配器的详细列表：

`ipconfig /all`

- 为一个网络适配器重新获取 IP 地址：

`ipconfig /renew {{适配器}}`

- 为一个网络适配器释放 IP 地址：

`ipconfig /release {{适配器}}`

- 清除所有 DNS 缓存：

`ipconfig /flushdns`
