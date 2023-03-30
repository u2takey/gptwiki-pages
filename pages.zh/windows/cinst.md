# cinst 
## chatgpt 
cinst是Chocolatey包管理器的命令之一，用于从Chocolatey源安装软件包。它是choco install的简称。

“cinst”的语法是：

cinst <package name>

其中，“<package name>”表示你要安装的软件包名称。

默认情况下，cinst将从默认的Chocolatey源安装软件包。你可以通过指定其他源来更改源站点。例如：

cinst <package name> -s <source>

其中，“<source>”表示源站点的URL地址。

除了安装软件包外，cinst还允许你在安装时指定特定的版本号，或执行其他一些命令选项，例如：

- --version：安装指定的版本。
- --force：强制安装指定软件包。
- --source：指定安装源。
- --installarguments：为在包安装期间传递给安装程序的任何参数定义单个参数或多个参数。
- --acceptlicense：自动接受许可协议。

总之，“cinst”是一个非常方便的命令，用于快速，安装软件包和应用程序。 

## tldr 
 
> 这是 `choco install` 命令的一个别名。
> 更多信息：<https://docs.chocolatey.org/en-us/choco/commands/install>.

- 原命令的文档在：

`tldr choco install`
