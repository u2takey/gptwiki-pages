# llvm-nm 
## chatgpt 
llvm-nm是一个命令行工具，用于显示LLVM二进制文件（包括目标文件、共享库、可执行文件等）中的符号表。

符号表是一个记录符号名称和相关信息（如符号类型和地址）的表格。符号在程序中扮演了重要的角色，它们代表着变量、函数、类、结构体等程序实体的名称和地址。

llvm-nm提供多种选项和参数，能够对符号表进行各种操作，例如：

- 显示符号表中的符号：该命令默认输出符号名称、类型和地址等信息。可以使用选项-f或-D来仅显示函数或仅显示数据符号。
- 查找符号表中的符号：可以通过在命令行中指定符号名称来直接查询符号信息。也可以使用选项-g或-u来仅查找全局符号或未定义符号。
- 修改符号表中的符号：使用选项-B或-S可以将符号表中的符号类型从本地变成全局或从弱符号变成强符号，也可以修改符号的名称和地址等信息。

总之，llvm-nm是一个功能强大的工具，可以帮助开发人员深入了解程序的符号表，并进行各种符号操作。 

## tldr 
 
> 这是 `nm` 命令的一个别名。

- 原命令的文档在：

`tldr nm`