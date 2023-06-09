# llvm-ar 
## chatgpt 
llvm-ar是一个可以创建、修改以及将文件从LLVM 归档文件中提取出来的命令行工具。这个工具在编译LLVM项目时经常使用。下面是关于这个命令的更详细的解释：

语法：llvm-ar [options] [operation] archive [members]

选项：

- -r：将文件添加到归档文件中。如果文件名已经存在，则将覆盖现有文件。
- -t：显示归档文件中的所有成员的名称列表。
- -x：从归档文件中提取指定的文件。可以指定多个文件名，以空格分隔。
- -c：使用指定的成员文件生成一个新的归档文件。可以指定多个成员文件名，以空格分隔。
- -s：将符号表添加到归档文件中。
- -v：在操作过程中显示详细信息。

操作：

- d：从归档文件中删除指定的成员。可以指定多个成员文件名，以空格分隔。
- m：将成员的时间戳和权限标志更新为归档文件中的新时间戳和权限标志。
- p：将指定的成员文件内容打印到标准输出。
- q：将文件添加到归档文件中。如果文件名已经存在，则不会覆盖现有文件。
- r：将文件添加到归档文件中。如果文件名已经存在，则将覆盖现有文件。
- s：将符号表添加到归档文件中或更新现有符号表。

指定归档文件：命令行中的第一个非选项参数是归档文件的名称。如果归档文件不存在，则将创建一个新的归档文件。

指定成员：归档文件中的成员文件可以直接通过文件名指定。文件名应该放在选项和操作之后。可以指定多个成员文件名，以空格分隔。

例子：

- 将多个文件添加到归档文件中：llvm-ar r libtest.a foo.o bar.o
- 从归档文件中提取指定的文件：llvm-ar x libtest.a foo.o
- 创建一个新的归档文件，并将指定的成员文件添加到其中：llvm-ar qc libnew.a foo.o bar.o 
- 删除归档文件中的指定文件：llvm-ar d libtest.a foo.o
- 显示归档文件中的所有成员的名称列表：llvm-ar t libtest.a 

## tldr 
 
> 这是 `ar` 命令的一个别名。

- 原命令的文档在：

`tldr ar`
