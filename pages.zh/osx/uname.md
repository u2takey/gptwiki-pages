# uname 
## chatgpt 
uname命令是一个Linux/Unix命令，用于显示当前操作系统的名称和版本信息。它的名称是Unix名称。在操作系统上输入uname命令时，将显示如下信息：

- Kernel Name：表示当前计算机运行的操作系统内核的名称（例如，Linux，FreeBSD，OpenBSD等）。
- Node Name：表示当前计算机的主机名。
- Kernel Release：表示当前计算机运行的操作系统内核的版本号。
- Kernel Version：表示当前计算机运行的操作系统内核的版本和补丁等详细信息。
- Machine：表示当前计算机的硬件架构（例如，x86，x86_64，sparc等）。

uname命令还有一些有用的选项，可以在输出中添加其他信息，如：

- -a 或 --all：显示完整系统信息。
- -m 或 --machine：显示硬件平台。
- -n 或 --nodename：显示网络主机名称。
- -r 或 --release：显示内核版本号。
- -s 或 --sysname：显示内核名称。
- -v 或 --version：显示内核版本。 

## tldr 
 
> 打印当前计算机及其上运行的操作系统的详细信息。
> 注意：有关操作系统的其他信息，请尝试使用 `sw-vers` 命令。
> 更多信息：<https://ss64.com/osx/uname.html>.

- 打印内核名称：

`uname`

- 打印系统架构和处理器信息：

`uname -mp`

- 打印内核名称、内核版本号和内核版本详细信息：

`uname -srv`

- 打印系统主机名：

`uname -n`

- 打印所有可用的系统信息：

`uname -a`
