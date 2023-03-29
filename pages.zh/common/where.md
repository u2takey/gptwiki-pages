# where 
## chatgpt 
命令：where

作用：在系统的环境变量路径中，搜索指定的可执行文件，并返回路径。

使用方法：在命令行窗口中输入 "where" 命令，后面加上指定的可执行文件的名称，如下所示：

where executable_file_name

其中 "executable_file_name" 是指要搜索的可执行文件的名称。

解释：

where 命令是 Windows 系统中的命令行工具，它用于在系统环境变量路径中搜索指定的可执行文件，并返回完整的路径。

Windows 操作系统的环境变量 PATH 包含了许多目录路径，存储了各种系统工具和软件的可执行文件路径。当在命令行中键入一个命令时，操作系统会在环境变量 PATH 中的路径中搜索对应的可执行文件。

例如，当你在命令行窗口中输入 "notepad" 命令时，Windows 操作系统将在 PATH 中指定的路径中搜索 notepad.exe 可执行文件，并执行它。where 命令可以帮助你查找该命令所在的路径。如果搜索到多个路径，则 where 命令将列出所有匹配的路径。如果没有找到可执行文件，则 where 命令将不会返回任何结果。

where 命令的主要优点是可以搜索包括环境变量 PATH 在内的多个路径。相比其他搜索文件的命令（如 dir 命令等），where 命令搜索的范围更广，可以找到更多的可执行文件。此外，where 命令也很容易使用，只需在命令行中输入文件名即可。 

## tldr 
 
> 报告所有已知的命令入口。
> 它可以是一个在`PATH`中的可执行文件，一个别名，或者一个 shell 內建命令。
> 更多信息：<https://zsh.sourceforge.io/Doc/Release/Shell-Builtin-Commands.html>.

- 报告所有已知命令入口：

`where {{command}}`
