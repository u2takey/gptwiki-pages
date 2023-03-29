# ip-route-list 
## chatgpt 
ip-route-list 命令用于查看系统中所有的路由表。它会显示出每一个路由表的详细信息，包括目标网络、网关、网卡名称、优先级等等。

具体用法：

$ ip route list

输出结果类似于：

default via 192.168.1.1 dev eth0 proto static 
192.168.1.0/24 dev eth0 proto kernel scope link src 192.168.1.100 metric 100 
192.168.2.0/24 via 192.168.1.2 dev eth0 proto static metric 100 
192.168.3.0/24 dev eth1 proto kernel scope link src 192.168.3.100 metric 101

解释：

- default 通过 eth0 网卡发送数据包，目标网关为 192.168.1.1，使用静态路由协议（proto static）。
- 192.168.1.0/24 通过 eth0 网卡发送数据包，源 IP 地址为 192.168.1.100，掩码为 24 位（相当于子网掩码为 255.255.255.0），路由优先级为 100。
- 192.168.2.0/24 通过 eth0 网卡发送数据包，目标网关为 192.168.1.2，使用静态路由协议，路由优先级为 100。
- 192.168.3.0/24 通过 eth1 网卡发送数据包，源 IP 地址为 192.168.3.100，掩码为 24 位，路由优先级为 101。

通过 ip-route-list 命令可以方便地查看路由表信息，并且可以根据需要进行调整和配置。 

## tldr 
 
> 这是 `ip-route-show` 命令的一个别名。

- 原命令的文档在：

`tldr ip-route-show`
