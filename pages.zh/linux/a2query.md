# a2query 
## chatgpt 
a2query是一个Apache web服务器的命令，它用于查询和输出与Apache2服务相关的信息，主要包括以下内容：

1. 查看Apache2模块状态：a2query -m [模块名称] 

该命令用于查看Apache2中各个模块的状态。其中，[模块名称]是可选参数，表示查看指定模块的状态，如果不指定模块名称，则会输出所有模块的状态。

2. 查看Apache2虚拟主机状态：a2query -s 

该命令用于查看Apache2中虚拟主机的状态，包括哪些虚拟主机正在运行、停止或已禁用。

3. 查看Apache2配置文件：a2query -f [配置文件名称] 

该命令用于查看Apache2的配置文件信息，其中，[配置文件名称]是可选参数，表示查看指定的配置文件信息，如果不指定配置文件名称，则会输出默认的Apache2配置文件信息。

总之，a2query命令是一个方便的工具，用于快速查询和输出Apache2服务相关的信息，从而帮助系统管理员更好地管理和维护Apache2服务器。 

## tldr 
 
> 在基于 Debian 的操作系统上查看 Apache 运行配置。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2query.html>.

- 列出启用的 Apache 模块：

`sudo a2query -m`

- 查看某个模块是否已安装：

`sudo a2query -m {{模块名}}`

- 列出已启用的虚拟主机：

`sudo a2query -s`

- 显示已启用的多进程模块：

`sudo a2query -M`

- 显示 Apache 版本：

`sudo a2query -v`
