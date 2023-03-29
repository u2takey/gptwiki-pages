# apt 
## chatgpt 
apt 是 Advanced Package Tool 的缩写，它是 Debian 和 Ubuntu 等 Linux 发行版中用来管理软件包的命令行工具。apt 可以帮助用户查找、安装、卸载和升级软件包，如：

- apt update：更新软件包列表，该命令会从软件源中下载最新的软件包列表，以便 apt 安装和升级软件包时使用。
- apt install：安装指定的软件包和其依赖项，如 apt install firefox。
- apt remove：卸载指定的软件包，如 apt remove firefox。
- apt upgrade：升级已安装的软件包，该命令会将系统中已安装的软件包与软件源中最新版本进行比较，并更新系统中的软件包。
- apt search：搜索符合指定名称或关键字的软件包，如 apt search apache2。
- apt list：显示已安装软件包的列表，如 apt list --installed。
- apt autoremove：自动删除已安装但不再需要的软件包，如 apt autoremove。

除了上述命令，apt 还有其他一些命令和选项，用户可以使用 apt --help 来查看完整的命令和选项列表。 

## tldr 
 
> 基于 Debian 的发行版上的软件包管理工具。
> 在 Ubuntu 16.04 及之后版本推荐用它代替 `apt-get` 。
> 更多信息：<https://manpages.debian.org/latest/apt/apt.8.html>.

- 更新可用软件包及其版本列表（推荐在运行其他 apt 命令前首先运行该命令）：

`sudo apt update`

- 查找指定软件包：

`apt search {{软件包}}`

- 显示关于指定软件包的信息：

`apt show {{软件包}}`

- 安装指定软件包或将指定软件包更新到最新版本：

`sudo apt install {{软件包}}`

- 移除指定软件包（使用 `purge` 同时移除其配置文件）：

`sudo apt remove {{软件包}}`

- 将所有已安装软件包更新到最新可用版本：

`sudo apt upgrade`

- 列出所有软件包：

`apt list`

- 列出已安装的软件包：

`apt list --installed`
