# a2dismod 
## chatgpt 
a2dismod 命令是 linux 系统中 Apache2 web服务器的一个命令，用于禁用（卸载）已安装的 Apache2 模块。它的具体用法如下：

a2dismod [模块名称]

其作用是将指定的模块从 Apache2 服务器中卸载，并从配置文件中删除相关的配置信息。有了这个命令，我们就可以轻松地对 Apache2 服务器的模块进行管理，方便地添加、卸载或管理相关的功能模块，保证 Apache2 服务器的性能和稳定性。 需要注意的是，这个命令需要运行在 root 或 sudo 权限下。 

## tldr 
 
> 在基于 Debian 的操作系统上禁用 Apache 模块。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2dismod.8.en.html>.

- 禁用模块：

`sudo a2dismod {{模块路径}}`

- 不显示信息性消息：

`sudo a2dismod --quiet {{模块路径}}`
