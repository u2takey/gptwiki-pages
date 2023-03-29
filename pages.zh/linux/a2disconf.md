# a2disconf 
## chatgpt 
a2disconf 命令是 Apache2 网页服务器的一个管理命令，用于从 Apache2 的默认配置中卸载或禁用一个或多个服务或虚拟主机配置文件。

具体来说，a2disconf 命令可以将指定的服务或虚拟主机配置文件从 Apache2 服务器的默认配置中卸载或禁用，使得 Apache2 服务器不再使用这些配置文件来启动或运行。

a2disconf 命令的语法格式如下：

a2disconf [选项] 配置文件名

其中，配置文件名指定要卸载或禁用的服务或虚拟主机配置文件的文件名。选项包括：

• --help：显示命令的帮助信息。

• --version：显示命令的版本信息。

使用 a2disconf 命令前，需要确保 Apache2 服务器已经安装并启动。另外，使用该命令对 Apache2 的默认配置进行修改可能会对服务器的运行产生影响，因此在使用前应当谨慎。 

## tldr 
 
> 在基于 Debian 的操作系统上禁用 Apache 配置文件。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2disconf.8.en.html>.

- 禁用配置文件：

`sudo a2disconf {{配置文件}}`

- 不显示信息性消息：

`sudo a2disconf --quiet {{配置文件}}`
