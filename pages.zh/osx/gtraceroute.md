# gtraceroute 
## chatgpt 
gtraceroute是一种图形化的traceroute工具，它可以帮助用户检查网络连接是否稳定，发现网络故障的原因，并帮助用户优化网络设置。其命令格式如下：

```
gtraceroute [选项] 主机名/IP地址
```

其中，主机名/IP地址是需要进行traceroute测试的目标地址。

常用选项说明如下：

- -h, --help        显示帮助信息
- -m, --max-ttl=N   设置最大的traceroute跳数，默认为30
- -n, --dont-resolve 不进行DNS反向解析
- -f, --first-ttl=N 开始traceroute测试时的TTL
- -s, --source=IP   指定源IP地址

在图形化界面中，gtraceroute会分别显示每个跳点的IP地址和域名以及ping的时间。用户可通过鼠标右键菜单选择跳点进一步进行traceroute测试或进行ping操作。 

## tldr 
 
> 这是 `-p linux traceroute` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux traceroute`
