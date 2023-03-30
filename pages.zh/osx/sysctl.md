# sysctl 
## chatgpt 
sysctl是一个系统管理命令，用于查询和修改Linux内核参数。

具体来说，sysctl命令有以下常用用途：

1. 查询系统参数

运行sysctl命令可查看当前系统的各种参数设置，例如内存大小、CPU架构、系统启动时间、网络设置等。

2. 修改内核参数

通过sysctl命令可以修改一些内核参数，例如TCP/IP协议栈的参数、进程调度策略等。

3. 保存参数设置

通过sysctl命令可以将当前的参数设置保存到配置文件中，使其在下次系统启动时自动生效。

例如，可以使用以下命令将TCP窗口大小调整为65535字节，并将该设置保存到配置文件中：

```
sysctl -w net.ipv4.tcp_window_scaling=1
sysctl -w net.ipv4.tcp_rmem="4096 87380 65535"
sysctl -w net.ipv4.tcp_wmem="4096 16384 65535"
echo "net.ipv4.tcp_window_scaling=1" >> /etc/sysctl.conf
echo "net.ipv4.tcp_rmem=4096 87380 65535" >> /etc/sysctl.conf
echo "net.ipv4.tcp_wmem=4096 16384 65535" >> /etc/sysctl.conf
```

总之，sysctl是一个强大的系统管理命令，可以帮助管理员调整系统参数以改善系统性能、优化网络连接等。 

## tldr 
 
> 访问内核状态信息。
> 更多信息：<https://ss64.com/osx/sysctl.html>.

- 显示所有可用变量及其值：

`sysctl -a`

- 显示 Apple 型号标识符：

`sysctl -n hw.model`

- 显示 CPU 模型：

`sysctl -n machdep.cpu.brand_string`

- 显示可用的 CPU 功能（MMX, SSE, SSE2, SSE3, AES, 等）：

`sysctl -n machdep.cpu.features`

- 设置一个可更改的内核状态变量：

`sysctl -w {{部分。可修改的变量}}={{值}}`
