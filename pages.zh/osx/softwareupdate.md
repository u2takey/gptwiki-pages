# softwareupdate 
## chatgpt 
softwareupdate命令用于在macOS系统上更新操作系统、应用程序和其他软件。它可以从苹果的软件更新服务器下载和安装最新版本的软件，可以通过终端或图形用户界面 (GUI) 进行使用。

以下是一些常见的软件更新命令选项和用法：

1. 查看可用更新：

在终端中输入"softwareupdate -l"，可以列出可用的更新和安装选项。这将列出所有可更新软件的名称和版本号。

2. 安装可更新的软件：

在终端中输入"softwareupdate -i [软件名称]"，可以安装指定的软件更新。如果要安装所有可用的更新，可以输入"softwareupdate -i -a"。

3. 禁用自动更新：

在终端中输入"sudo softwareupdate --schedule off"，可以禁用自动更新。如果要重新启用自动更新，可以输入"sudo softwareupdate --schedule on"。

4. 查看更新历史：

在终端中输入"softwareupdate --history"，可以查看已安装的更新历史记录。

5. 强制升级：

在终端中输入"sudo softwareupdate --install -all --force"，可以强制安装所有可用的软件更新。

注意事项：

在使用softwareupdate命令时，需要具有管理员权限，即需要在命令前面加上"sudo"。此外，在更新过程中，可能需要输入密码或确认。更新过程也可能需要一些时间，取决于软件包的大小和下载速度。 

## tldr 
 
> 通过命令行更新 macOS 应用商店中应用程序的工具。
> 更多信息：<https://ss64.com/osx/softwareupdate.html>.

- 列出所有可用的更新：

`softwareupdate -l`

- 下载并安装所有更新：

`softwareupdate -ia`

- 下载并安装所有推荐的更新：

`softwareupdate -ir`

- 下载并安装特定的应用程序：

`softwareupdate -i {{更新应用程序名}}`
