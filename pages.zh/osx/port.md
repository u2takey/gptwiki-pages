# port 
## chatgpt 
port命令是Mac系统中用于管理软件包和依赖项的工具，类似于Linux的apt-get或yum命令。它使用MacPorts软件包管理器，可以让用户轻松下载、安装、更新和删除软件包。

常用的port命令有：

1. `port search [软件包名]`：搜索可用的软件包列表；
2. `port install [软件包名]`：安装指定的软件包及其所有依赖项；
3. `port uninstall [软件包名]`：卸载指定的软件包及其所有依赖项；
4. `port list installed`：列出所有已安装的软件包；
5. `port outdated`：列出所有已安装但版本不是最新的软件包；
6. `port upgrade outdated`：将所有已安装但版本不是最新的软件包升级到最新版本。

除此之外，port命令还支持其他一些高级选项和参数，比如指定软件包版本、安装软件包的指定变体（variants）等。需要注意的是，使用port命令需要管理员权限。 

## tldr 
 
> macOS 包管理器软件（类似 brew）。
> 更多信息：<https://www.macports.org>.

- 搜索包：

`port search {{搜索的包名}}`

- 安装软件包：

`sudo port install {{报名}}`

- 列出已安装的软件包：

`port installed`

- 更新 port 自身，并获取可用包的最新列表：

`sudo port selfupdate`

- 升级过时的软件包：

`sudo port upgrade outdated`

- 删除已安装的软件包的旧版本：

`sudo port uninstall inactive`
