# cc 
## chatgpt 
cc命令在Linux中是一个C语言编译器命令，意为C Compiler。它是GNU Compiler Collection（GCC）中的一员，用于将C语言源代码编译为可执行文件。

cc命令常常用于编译C语言程序。其语法格式为：

cc [选项] 文件名

其中，选项有很多种，常用的包括：

- -o：指定编译出来的可执行文件的文件名；
- -c：只编译生成目标文件，不进行链接；
- -E：进行预处理，输出预处理结果。

例如，编译一个名为test.c的C语言程序，可以使用cc命令：

cc test.c -o test

这条命令将会编译test.c文件，并将生成的可执行文件命名为test。然后，可以使用./test命令运行该程序。

总之，cc命令可以帮助开发人员将C语言源代码编译成可执行文件，是Linux系统中非常重要的命令之一。 

## tldr 
 
> 这是 `gcc` 命令的一个别名。
> 更多信息：<https://gcc.gnu.org>.

- 原命令的文档在：

`tldr gcc`
