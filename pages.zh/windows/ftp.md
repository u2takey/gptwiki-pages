# ftp 
## chatgpt 
ftp命令是一种用于在计算机间传输文件的协议和实用工具。它可以用于从一个计算机向另一个计算机传输文件或从一个计算机复制文件。下面是一些常用的ftp命令及其作用：

1. ftp domainname/ipaddress：打开一个新的ftp连接，并连接到一个远程计算机（可以是域名或IP地址）。

2. anonymous：用匿名方式登录ftp会话。

3. user username：用给定的用户名登录ftp会话。

4. cd directory：改变服务器上的当前目录。

5. lcd directory：改变本地计算机上的当前目录。

6. get filename：从服务器下载给定的文件。

7. put filename：将本地计算机上的文件上传到服务器。

8. ls：在服务器上列出当前目录中的文件。

9. quit：结束当前ftp会话。

总之，ftp命令是一种用于在计算机和服务器之间传输文件的工具和协议，具有访问和传输权限的登录和控制过程，并且包括一组文件传输命令。 

## tldr 
 
> 在本地和远程 FTP 服务器之间交互式传输文件。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/ftp>.

- 交互式连接一个远程的 FTP 服务：

`ftp {{主机名}}`

- 匿名登录：

`ftp -A {{主机名}}`

- 初始连接时禁用自动登录：

`ftp -n {{主机名}}`

- 运行包含 FTP 命令列表的文件：

`ftp -s:{{文件的路径}} {{主机名}}`

- 下载多个文件（通配符表达式）：

`mget {{*.png}}`

- 上传多个文件（通配符表达式）：

`mput {{*.zip}}`

- 在远程服务器上删除多个文件：

`mdelete {{*.txt}}`

- 显示详细的帮助：

`ftp --help`
