# doskey 
## chatgpt 
doskey是Windows中的一个命令行工具，它用于创建、显示、编辑、重定向以及删除命令行历史中的命令。它的主要功能是将一个命令行命令的名字与一段脚本或者一串代码相关联。

doskey有多个参数，这里列出一些主要的参数及其作用：

- /history：列出命令行历史记录。
- /listsize：设置命令行历史记录中最大的行数。
- /insert：将一个新的命令添加到历史记录中。
- /macrofile：导入宏文件。
- /reinstall：重新安装DOSKEY.EXE。

使用doskey命令，可以方便地自定义属于自己的命令行小脚本，比如将一个复杂的命令行脚本绑定到一个简单易记的命令别名上。这样，无论何时需要运行这个脚本，只需要输入这个别名，就可以轻松地执行该脚本。doskey还有很多其他的用法，可以根据不同的需求对其进行更深入的学习和了解。 

## tldr 
 
> 管理宏，Windows 命令和命令行。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/doskey>.

- 列出可用的宏：

`doskey /macros`

- 创建一个新的宏：

`doskey {{宏的名称}} = "{{命令}}"`

- 为指定可执行文件创建新的宏：

`doskey /exename={{可执行文件名}} {{宏的名称}} = "{{命令}}"`

- 删除一个宏：

`doskey {{宏的名称}} =`

- 列出所有储存在内存中的命令：

`doskey /history`

- 将宏保存到文件以便于移植：

`doskey /macros > {{保存宏的文件名}}`

- 从文件中加载宏：

`doskey /macrofile = {{保存宏的文件名}}`
