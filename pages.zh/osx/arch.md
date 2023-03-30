# arch 
## chatgpt 
arch命令是一个Linux命令，用于显示当前操作系统的处理器架构或体系结构。该命令没有任何参数，应用时直接在终端中输入arch即可。

它将输出当前处理器的体系结构，如x86，x86_64，ARM等等。这些信息对于调试和在不同的体系结构上运行二进制程序非常有用。此外，arch命令也可用于确定适当的包，以便下载特定于架构的软件包。

例如，若你使用的是基于x86_64体系结构的Linux系统，那么在终端中输入arch命令时，将会输出x86_64。类似地，如果你使用的是基于ARM体系结构的Linux系统，那么将会输出ARM。 

## tldr 
 
> 显示系统架构的名称，或者在不同的架构下运行命令。
> 另见 `uname`.
> 更多信息：<https://www.unix.com/man-page/osx/1/arch/>.

- 显示系统的架构：

`arch`

- 使用 x86_64 来运行一个命令：

`arch -x86_64 {{命令}}`