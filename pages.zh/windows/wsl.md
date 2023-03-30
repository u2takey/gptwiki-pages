# wsl 
## chatgpt 
wsl是Windows Subsystem for Linux（Windows 子系统 Linux）的缩写，是Windows 10操作系统独有的功能之一。它允许 Windows 用户直接在 Windows 系统上运行 Linux 环境，因为其实际上是真正的 Linux 内核运行在 Windows 系统上。用户可以在 Windows 系统中使用以往只能在 Linux 系统上使用的命令行工具和应用程序。通过 wsl 命令，用户可以管理其安装和运行的 WSL 子系统，包括启动、停止、升级和配置等操作。部分 wsl 命令及其功能如下：

- wsl --list：列出当前安装的 WSL 子系统。
- wsl --set-default-version：设置默认的 WSL 子系统版本。
- wsl --shutdown：停止运行中的 WSL 子系统。
- wsl --upgrade：升级 WSL 子系统版本。
- wsl --import：从一个.tar 文件导入 WSL 子系统。
- wsl --export：导出指定 WSL 子系统到一个.tar 文件。
- wsl --exec：运行指定的命令行，类似于在 Linux 终端中输入命令。

总之，wsl 命令使用户能够在 Windows 操作系统下更方便地访问 Linux 环境及其相关应用程序，提高了跨平台的兼容性和应用程序的可用性。 

## tldr 
 
> 从命令行管理适用于 Linux 的 Windows 子系统。
> 更多信息：<https://learn.microsoft.com/windows/wsl/reference>.

- 启动 Linux Shell（在默认发行版中）：

`wsl {{shell_命令}}`

- 在不使用 Shell 的情况下运行 Linux 命令：

`wsl --exec {{命令}} {{命令参数}}`

- 指定特定的发行版：

`wsl --distribution {{发行版}} {{shell_命令}}`

- 列出所有可用发行版：

`wsl --list`

- 将发行版导出到 .tar 文件：

`wsl --export {{发行版}} {{路径/distro_fs.tar}}`

- 从 .tar 文件导入发行版：

`wsl --import {{发行版}} {{路径/安装位置}} {{路径/distro_fs.tar}}`

- 更改指定发行版的版本：

`wsl --set-version {{发行版}} {{版本}}`

- 关闭适用于 Linux 的 Windows 子系统：

`wsl --shutdown`
