# getmac 
## chatgpt 
getmac是Windows系统下的一条命令，用于显示计算机的MAC地址（Media Access Control Address）。

在计算机网络中，MAC地址是一个唯一的标识符，它在数据链路层上用于标识网络中不同的设备。每个网络设备都有自己的MAC地址，包括电脑、路由器、交换机、网卡等等。MAC地址由48个二进制数位组成，通常以十六进制表示。

使用getmac命令可以获取计算机当前连接到网络上的所有设备的MAC地址，包括本地以太网卡、Wireless网卡、虚拟网卡等等。

具体使用方法：在命令行窗口中输入getmac，按下回车键，即可显示计算机所有网络设备的MAC地址。可加上参数/v /fo list，将结果输出为列表格式。 

## tldr 
 
> 显示系统的 MAC 地址。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/getmac>.

- 显示当前系统的 MAC 地址：

`getmac`

- 以特定格式显示详细信息：

`getmac /fo {{table|list|csv}}`

- 排除输出列表中的标题：

`getmac /nh`

- 显示一个远程主机的 MAC 地址：

`getmac /s {{主机名}} /u {{用户名}} /p {{密码}}`

- 详细显示 MAC 地址信息：

`getmac /v`

- 显示详细的帮助信息：

`getmac /?`
