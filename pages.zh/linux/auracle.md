# auracle 
## chatgpt 
很抱歉，auracle 不是标准的 Linux 命令，它是 Arch Linux 操作系统中的 AUR（Arch User Repository）助手。

AUR 是 Arch Linux 上的一种社区维护的软件源，提供了许多用户在 Arch Linux 中需要的软件包，auracle 则是一种用于管理和查询 AUR 软件包的命令行界面工具。

以下是 auracle 常用的命令和功能：

1. `auracle search`：搜索 AUR 软件包。
2. `auracle info`：查看 AUR 软件包的详细信息，包括版本、依赖关系等。
3. `auracle download`：下载 AUR 软件包。
4. `auracle build`：构建和安装 AUR 软件包。
5. `auracle checkupdates`：检查 AUR 软件包的更新情况。
6. `auracle upgrade`：升级 AUR 软件包。

可以使用 `man auracle` 命令查看完整的 auracle 手册和用法说明。 

## tldr 
 
> 用来和 Arch Linux 用户仓库交互的命令行工具，这个仓库通常被称作 AUR.
> 更多信息：<https://github.com/falconindy/auracle>.

- 显示符合一个正则表达式的 AUR 包：

`auracle search '{{regular_expression}}'`

- 显示 AUR 包列表的包信息，包名以一个单独的空格分隔：

`auracle info {{package1}} {{package2}}`

- 显示 AUR 包列表的 `PKGBUILD` 文件（编译信息），包名以一个单独的空格分隔：

`auracle show {{package1}} {{package2}}`

- 显示已安装 AUR 包的更新：

`auracle outdated`
