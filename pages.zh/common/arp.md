# arp 
## chatgpt 
arp（Address Resolution Protocol）命令用于获取和管理本地计算机或网络中的 ARP（Address Resolution Protocol）缓存条目。ARP协议是用于将IP地址解析为MAC地址的协议。

常用选项包括：

- -a：显示全部缓存的ARP表信息
- -d：删除指定IP地址对应的ARP缓存
- -s：手动添加ARP缓存，可以将IP地址和MAC地址进行绑定

例如，要显示本机的ARP缓存表信息，可以使用以下命令：

```
arp -a
```

要手动添加一个ARP缓存，可以使用以下命令：

```
arp -s <ip_address> <mac_address>
```

其中，`<ip_address>`是要绑定的IP地址，`<mac_address>`是要绑定的MAC地址。 

## tldr 
 
> 显示和操作系统的 ARP 缓存。
> 更多信息：<https://manned.org/arp>.

- 显示当前的 ARP 表：

`arp -a`

- 清除整个缓存：

`sudo arp -a -d`

- 删除特定条目：

`arp -d {{地址}}`

- 创建指定条目：

`arp -s {{地址}} {{MAC 地址}}`
