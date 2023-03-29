# flatpak 
## chatgpt 
flatpak 是一种软件包管理工具，用于在 Linux 系统上安装、管理和更新软件应用。与传统的 Linux 软件管理工具（如 apt，yum，pacman 等）不同，flatpak 可以不依赖于特定的 Linux 发行版或软件库，使您可以使用相同的应用程序包在多个不同的 Linux 系统上运行软件。

flatpak 的命令用于安装、展示、运行和更新 flatpak 软件包。以下是一些最常用的 flatpak 命令：

- `flatpak install <app_name>`：安装指定的 flatpak 软件包。
- `flatpak list`：列出当前系统中已经安装的 flatpak 软件包。
- `flatpak update`：更新当前系统中所有已安装的 flatpak 软件包。
- `flatpak run <app_name>`：启动指定的 flatpak 应用程序。
- `flatpak uninstall <app_name>`：删除指定的 flatpak 软件包。
- `flatpak info <app_name>`：显示关于指定 flatpak 软件包的详细信息，例如版本号、依赖项等。

flatpak 还提供了其他高级命令和选项，可用于处理扩展仓库、批量安装和更新、设置运行时环境等特殊任务。对于熟悉 Linux 系统管理和软件包管理的用户来说，使用 flatpak 应该会比较容易。 

## tldr 
 
> 构建、安装和运行 Flatpak 应用和运行时。
> 更多信息：<https://docs.flatpak.org/en/latest/flatpak-command-reference.html#flatpak>.

- 运行已安装应用：

`flatpak run {{应用名}}`

- 从远程源安装应用：

`flatpak install {{远程源名}} {{应用名}}`

- 列出所有应用和运行时：

`flatpak list`

- 更新所有已安装的应用和运行时：

`flatpak update`

- 添加远程源：

`flatpak remote-add --if-not-exists {{远程源名}} {{远程源网址}}`

- 列出所有已配置的远程源：

`flatpak remote-list`

- 移除一个已安装的应用程序：

`flatpak remove {{应用名}}`

- 显示一个已安装的应用程序的信息：

`flatpak info {{应用名}}`
