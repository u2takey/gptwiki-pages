# choco uninstall 
## chatgpt 
命令 "choco uninstall" 是 Chocolatey Package Manager 的一个命令。它用于卸载已安装的软件包。

当你在 Windows 系统中使用 Chocolatey 安装了软件包后，你可能需要卸载它们，以释放磁盘空间或修复系统问题。 "choco uninstall" 命令帮助你轻松地卸载这些软件包。

使用 "choco uninstall" 命令时，你需要提供要卸载的软件包的名称。你还可以使用其他选项和参数来协助执行卸载操作。例如：

- "--all" 选项可以卸载所有已安装的软件包，而不需要一个个输入它们的名称。
- "--yes" 选项可以直接确认所有询问，跳过确认过程。
- "--force" 选项可以强制卸载软件包，即使它们正在被使用或其他进程正在运行。

总之，"choco uninstall" 是 Chocolatey Package Manager 工具中可用的一项功能，帮助用户轻松地卸载已安装的软件包。 

## tldr 
 
> 使用 Chocolatey 卸载一个或多个包。
> 更多信息：<https://chocolatey.org/docs/commands-uninstall>.

- 卸载一个或多个用空格分隔的软件包：

`choco uninstall {{包名 『包名』 ..}}`

- 卸载一个指定版本的包：

`choco uninstall {{包名}} --version {{版本号}}`

- 自动确认所有提示：

`choco uninstall {{包名}} --yes`

- 卸载时同时删除其所有的依赖：

`choco uninstall {{包名}} --remove-dependencies`

- 卸载全部包：

`choco uninstall all`
