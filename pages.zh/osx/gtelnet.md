# gtelnet 
## chatgpt 
gtelnet是一个用于在Linux和Unix系统中与远程主机进行交互的命令行工具。它基于telnet协议，允许用户在命令行界面中远程访问和管理主机。 

常用的参数和用法如下：

用法：gtelnet [选项] [主机名] [端口号]

选项：

-4 : 强制使用IPv4地址。
-6 : 强制使用IPv6地址。
-a : 将后续输入的用户名和密码都自动化输入。
-E : 禁止在运行控制终端（tty）时发送环境变量。
-e : 使用 Escape Character 作为转义字符。
-k : 允许输入 BACKSPACE 键起作用。
-l 用户名 : 指定的登录用户名。
-n : 使用 nl (newline) 代替 CR-LF (carriage return-linefeed)。
-p 端口号 : 指定端口号。
-R : 支持记录，并将其记录到指定的文件中。
-t : 强制使用 telnet 协议。
-V : 显示版本信息。
-w 毫秒 : 设置通信超时时间。
-x 表示不使用 telnet 协议。
-Z : 使用 telnet 数据压缩。
 

示例：

1. gtelnet 192.168.1.1 
 连接到远程主机 192.168.1.1。

2. gtelnet -l john 192.168.1.1 23
 用指定的用户名 john 连接到端口号 23 上运行的远程主机 192.168.1.1。

3. gtelnet -p 2022 -4 -e 10.0.0.1
 以 IPv4 地址 10.0.0.1 连接到远程主机，使用 telnet 协议，使用 Escape Character 作为转义字符，连接端口号是 2022。

4. gtelnet -E -n 192.168.1.1
 禁止在运行控制终端的情况下发送环境变量，使用 nl 代替 CR-LF，连接到远程主机 192.168.1.1。 

## tldr 
 
> 这是 `-p linux telnet` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux telnet`
