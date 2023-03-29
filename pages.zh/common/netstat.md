# netstat 
## chatgpt 
netstat是一个网络工具，用于显示当前主机的网络连接信息、路由表和网络接口等信息。

具体使用方法如下：

1. netstat -a：显示所有已建立的连接和侦听状态的端口。
2. netstat -n：以数字形式显示地址和端口。
3. netstat -b：显示每个进程的执行时的可执行文件名。
4. netstat -o：显示每个连接的进程ID。
5. netstat -p：显示与协议相关的连接信息。
6. netstat -r：显示路由表。
7. netstat -s：显示统计信息。 

示例：netstat -a 显示所有已建立的连接和侦听状态的端口。

输出结果包括本地地址、远程地址、协议类型、状态和PID等信息。示例输出如下：

```
Active Internet connections (including servers)
Proto Recv-Q Send-Q Local Address               Foreign Address             State           PID/Program name
tcp        0      0 0.0.0.0:http                0.0.0.0:*                   LISTEN      4092/lighttpd
tcp        0      0 192.168.1.5:ssh             192.168.1.37:35445          ESTABLISHED 10645/sshd: root@pts
tcp6       0      0 :::80                      :::*                        LISTEN      4092/lighttpd
tcp6       0      0 ::1:631                    :::*                        LISTEN      1085/cupsd
udp        0      0 0.0.0.0:39439               0.0.0.0:*                               1559/dhclient
udp        0      0 0.0.0.0:mdns                0.0.0.0:*                               1224/avahi-daemon
```

从输出结果中可以看到当前主机上所有的网络连接信息，包括TCP/UDP协议、本地地址、远程地址/端口、状态和进程ID等信息。 

## tldr 
 
> 显示与网络相关的信息，如打开的连接、打开的套接字端口等。
> 更多信息：<https://man7.org/linux/man-pages/man8/netstat.8.html>.

- 列出所有端口：

`netstat -a`

- 列出所有被侦听端口：

`netstat -l`

- 列出侦听的 TCP 端口：

`netstat -t`

- 显示监听给定协议监听的 PID 和程序名：

`netstat -p {{协议}}`

- 打印路由表：

`netstat -nr`
