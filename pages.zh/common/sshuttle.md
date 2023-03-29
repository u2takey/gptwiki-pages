# sshuttle 
## chatgpt 
sshuttle 是一个使用 SSH 进行 VPN 并绕过防火墙的工具。它可以将所有 TCP 流量通过 SSH 通道发送到远程主机，从而实现访问远程服务器上的网络服务。它在本地机器上创建一个虚拟的 TUN 网络接口，并使用 SSH 连接通信，从而可以访问远程主机上的网络资源，从而实现绕过防火墙限制的功能。

sshuttle 的命令具体如下：

sshuttle [OPTIONS] [HOSTS] [OPTIONS]
 
其中，OPTIONS 包括以下内容：
 
-h, --help               显示帮助信息
-v, --version            显示 sshuttle 版本信息
--dns-hosts FILE         使用指定的 DNS 文件
--dns-port PORT          替代 DNS 端口 (默认是 53)
--method NAME            传输方法 (默认是 nat)
--pidfile FILE           写入 pid 文件
--ssh-cmd CMD            使用指定的 ssh 命令连接主机
--sudo                  使用 sudo 运行 sshuttle
 
HOST 是需要访问的远程主机列表，可以是 IP 或主机名。

sshuttle 支持的几种模式包括：

1. 代理：可以设置为代理，在本地机器上运行 sshuttle 并隧道代理流量到远程机器上，绕过防火墙限制。具体命令示例如下：

sshuttle -r username@remote_host 0/0 

其中，-r 参数用于指定远程主机的地址和 SSH 登录凭据。

2. SSH 隧道：可以将远程主机上特定服务的流量通过本地机器的 sshuttle 隧道发送，从而实现访问远程主机上的服务。具体命令示例如下：

sshuttle --dns -r username@remote_host 10.0.0.0/8
 

其中，10.0.0.0/8 是需要访问的远程主机列表。

总而言之，sshuttle 是一种非常实用的工具，可以帮助用户更加灵活、高效地使用 SSH 连接远程主机，并在绕过防火墙限制的情况下访问远程主机上的网络资源。 

## tldr 
 
> 通过 ssh 连接传输流量的透明代理服务器。
> 不需要管理员或远程 ssh 服务器上的任何特殊设置。
> 更多信息：<https://manned.org/sshuttle>.

- 通过远程 ssh 服务器转发所有 IPv4 TCP 流量：

`sshuttle --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}}`

- 转发所有 IPv4 TCP 和 DNS 流量：

`sshuttle --dns --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}}`

- 使用 tproxy 方法转发所有 IPv4 和 IPv6 流量：

`sudo sshuttle --method=tproxy --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}} {{::/0}} --exclude={{你本地 IP 地址}} --exclude={{SSH 服务器的 IP 地址}}`
