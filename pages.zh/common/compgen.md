# compgen 
## chatgpt 
compgen命令是一个内置的Bash命令，用于列出某些东西的匹配模式的选项。其语法为：

compgen [option] [word]

其中，

- option：可选参数，可以是以下任何一种（多个选项可以组合在一起）：

  - `-a`：列出所有别名(alias)
  - `-b`：列出所有Bash函数(functions)
  - `-c`：列出所有Shell命令(commands)
  - `-d`：列出所有目录(directory)
  - `-e`：列出所有Shell变量(variables)
  - `-f`：列出所有文件(file)
  - `-g`：列出所有负责管理作业的进程(process group)的ID
  - `-j`：与-a选项相同，但也包括shell函数（shell functions）
  - `-k`：与-b选项相同，但也包括shell函数（shell functions）
  - `-s`：列出所有Shell关键字(keywords)
  - `-u`：列出所有未附加到文件描述符或重定向到单词表的变量名
  
- word：可选参数，它是作为要匹配的模式的基础的字符串。如果省略，word的默认值为“*”。

compgen被广泛用于创建自定义Shell命令补全，它可以列出所有与要补全的内容相关的选项和匹配模式。例如，您可以键入“compgen -c”和按下Tab键，它将列出您可以在当前情况下使用的所有Shell命令。 

## tldr 
 
> 用于在 bash 中自动完成的内置命令，按两次 tab 键即可调用该命令。
> 更多信息：<https://www.gnu.org/software/bash/manual/bash.html#index-compgen>.

- 显示所有可以执行的命令：

`compgen -c`

- 列出所有别名：

`compgen -a`

- 列出所有可以运行的函数：

`compgen -A function`

- 列出所有 shell 的保留关键字：

`compgen -k`

- 查看以 'ls' 开头的所有可用命令和别名：

`compgen -ac {{ls}}`
