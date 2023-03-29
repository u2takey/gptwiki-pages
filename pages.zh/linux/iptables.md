# iptables 
## chatgpt 
iptables 是一个用于配置 Linux 操作系统中的 IPv4 和 IPv6 的防火墙工具。它允许用户配置系统的入站和出站数据包以防止未授权访问和网络攻击。

iptables 命令有很多选项和参数，这里列举一些常用的：

1. -A,--append：在规则列表的末尾添加一条新规则。

2. -D,--delete：删除规则列表中的一条或多条规则。

3. -I,--insert：在规则列表的指定位置插入一条新规则。

4. -L,--list：列出当前规则列表。

5. -F,--flush：清空规则列表。

6. -N,--new-chain：创建一个新的用户定义的规则链。

7. -P,--policy：设置默认的规则链策略。

8. -R,--replace：用新的规则替换旧的规则。

9. -S,--save：将规则列表保存到文件中。

10. -Z,--zero：将规则列表的包计数器和字节计数器清零。

用户可以使用 iptables 命令来配置多种防火墙规则，例如：

1. 设置防火墙的默认策略。

2. 允许或拒绝特定IP地址访问系统。

3. 允许或拒绝特定端口的入站或出站数据包。

4. 允许或拒绝通过协议类型（TCP，UDP 或 ICMP）的访问请求。

5. 允许或拒绝某些网络服务或协议的访问。

6. 拦截或转发数据包。

iptables 命令需要插件支持，插件会根据用户的输入生成一些规则，这些规则会被写入到 iptables 防火墙配置文件中。iptables 的防火墙配置文件通常位于 /etc/sysconfig/iptables 或 /etc/iptables.rules 目录下，如果想要修改防火墙设置，往往需要编辑这些配置文件。 

## tldr 
 
> 可用于配置 Linux 内核防火墙提供的过滤表、规则链和规则的程序。
> 更多信息：<https://www.netfilter.org/projects/iptables/>.

- 查看过滤表的规则链、规则以及数据包/字节计数器：

`sudo iptables -vnL`

- 设定规则链策略规则：

`sudo iptables -P {{规则链}} {{规则}}`

- 追加规则到 IP 的规则链策略：

`sudo iptables -A {{规则链}} -s {{ip}} -j {{规则}}`

- 追加规则到 IP 的规则链策略（考虑协议与端口）：

`sudo iptables -A {{规则链}} -s {{ip}} -p {{协议}} --dport {{端口}} -j {{规则}}`

- 删除规则链中的规则：

`sudo iptables -D {{规则链}} {{规则所在行号}}`

- 将指定过滤表的 iptables 配置保存到文件中：

`sudo iptables-save -t {{过滤表名}} > {{iptables_文件路径}}`

- 从文件中还原 iptables 配置：

`sudo iptables-restore < {{iptables_文件路径}}`
