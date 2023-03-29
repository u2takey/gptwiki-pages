# acyclic 
## chatgpt 
acyclic 是一个命令行工具，用于检测和报告指定文件中的循环依赖。它通常用于软件开发的过程中，以确保代码库中没有循环依赖的情况，否则会导致程序在解析依赖关系时出现问题。

明确的说， acyclic 命令通过分析指定文件中的依赖关系图，并检测是否存在循环依赖的情况。如果检测到了循环依赖，则 acyclic 将在终端中显示错误消息，并给出相应的建议。如果没有发现循环依赖，那么 acyclic 命令就不会发出任何提示。

在 Unix/Linux 操作系统的环境中，acyclic 命令是一个通用的工具，可以用来检测任何类型的文本文件和脚本语言。它也可以用于检测其他类型的文件，如 Makefile 等。

例如，可以使用以下命令检测 C/C++文件中的循环依赖：

`acyclic path_to_file.cpp`

则 acyclic 将解析 path_to_file.cpp 文件中的所有依赖项，并检查是否存在循环依赖。如果存在循环依赖，则会在终端中显示一个错误消息，否则不会出现任何提示。 

## tldr 
 
> 通过反转一些边来使有向图无环。
> Graphviz 过滤器：`acyclic`、`bcomps`、`comps`、`edgepaint`、`gvcolor`、`gvpack`、`mingle`、`nop`、`sccmap`、`tred` 和 `unflatten`。
> 更多信息：<https://graphviz.org/pdf/acyclic.1.pdf>.

- 通过反转一些边来使有向图无环：

`acyclic {{路径/到/输入.gv}} > {{路径/到/输出.gv}}`

- 打印出一个图是无环的、有环的还是无向的，不产生输出图：

`acyclic -v -n {{路径/到/输入.gv}}`

- 显示 `acyclic` 的帮助：

`acyclic -?`
