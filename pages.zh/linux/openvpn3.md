# openvpn3 
## chatgpt 
Linux命令openvpn3是OpenVPN的第三代CLI客户端命令。OpenVPN是一个开源VPN协议，可以为私人和商业VPN连接提供安全的远程访问。openvpn3命令提供的命令选项和参数用于输入OpenVPN配置文件的路径、用户名、密码、证书和密钥等等。一些常用选项包括：

- config：指定OpenVPN配置文件的路径。
- auth-user-pass：指定用于身份验证的用户名和密码文件路径。
- cert：指定OpenVPN客户端证书的路径。
- key：指定OpenVPN客户端密钥的路径。
- remote：指定OpenVPN服务端的IP地址或主机名和端口号。
- log：指定日志文件的路径。

使用openvpn3命令可以方便地启动、停止和管理OpenVPN VPN连接，同时也提供了一些高级选项和配置，使用户可以自定义安全设置和网络协议。 

## tldr 
 
> OpenVPN 3 Linux 客户端。
> 更多信息：<https://community.openvpn.net/openvpn/wiki/OpenVPN3Linux>.

- 打开一个新的 VPN 会话：

`openvpn3 session-start --config {{路径/到/config.conf}}`

- 列出已建立的会话：

`openvpn3 sessions-list`

- 断开当前建立的以给定配置开始的会话：

`openvpn3 session-manage --config {{路径/到/config.conf}} --disconnect`

- 导入 VPN 配置：

`openvpn3 config-import --config {{路径/到/config.conf}}`

- 列出导入的配置：

`openvpn3 configs-list`
