# which 
## chatgpt 
which 命令用于查找并显示给定命令的可执行文件的完整路径。它可以用于确定哪个安装的软件提供了给定命令。例如，如果您使用 which python 命令，则可以找到 Python 解释器的完整路径。

该命令在 Linux 和 macOS 中可用，但在 Windows 中不可用。在 Windows 中，可以使用 where 命令来执行类似的操作。 

## tldr 
 
> 在用户的`PATH`中寻找可执行文件的路径。
> 更多信息：<https://manned.org/which>.

- 在`PATH`中寻找可执行文件并打印第一个匹配的结果：

`which {{executable}}`

- 如果有多个匹配结果则打印所有结果：

`which -a {{executable}}`
