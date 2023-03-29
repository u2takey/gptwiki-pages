# addr2line 
## chatgpt 
Linux 命令 "addr2line" 是用来将程序中的内存地址转换为源代码的行号和文件名的工具。它一般用于调试程序时，定位代码中的错误或异常。

addr2line 命令的语法格式为：

addr2line [-a|--addresses] [-b bfdname|--target=bfdname] [-C|--demangle[=style]] [-e filename|--exe=filename] [-f|--functions] [-i|--inlines] [-j section|--section=section] [-s|--basename] [-H|--help] [--version] [addr1] [addr2] [...]

选项说明：

-a, --addresses：给出每个地址的偏移量和地址。

-b bfdname, --target=bfdname：指定二进制文件使用的BFD库名称。

-C, --demangle[=style]：将C++函数名还原，可选风格有：auto, no, gnu, lucid，arm等。

-e filename, --exe=filename：将地址解释为来自的二进制文件。

-f, --functions：给出每个地址的函数名称。

-i, --inlines：显示调用带有行内函数的函数时，地址的行内部分。

-j section, --section=section：解析指定段的地址。

-s, --basename：不显示每个文件名的完整路径。

-H, --help：显示帮助信息。

--version：显示版本信息。

addr1, addr2…：需要转换行号和文件名的内存地址。

使用示例：

1. 查看某个二进制程序的版本号

addr2line --version

2. 将地址转换为函数名和行数

addr2line -fie /path/to/binary 0x8001cfa

3. 将地址解释为来自另一个二进制文件

addr2line -f -e /path/to/another-binary 0x8001cfa

4. 将地址转换为调用它的函数的名称

addr2line -Cfie /path/to/binary 0x8001cfa

5. 查看某个地址指向的文件和行号

addr2line -Cfe /path/to/binary 0x8001cfa

注意事项：

1. 需要相应的调试符号文件才能正确解析地址。

2. 函数名可能被编译器压缩，需要使用 "-C" 选项还原函数名称。

3. 文件名和行号可能不准确，因为编译器可能对源代码进行了优化和变形。 

## tldr 
 
> 将二进制文件地址转换成文件名和行数。
> 更多信息：<https://manned.org/addr2line>.

- 显示可执行文件的指令地址对应源代码的文件名和行数：

`addr2line --exe={{可执行文件路径}} {{地址}}`

- 显示函数名、文件名和行数：

`addr2line --exe={{可执行文件路径}} --functions {{地址}}`

- 将 C++ 代码函数名符号重组：

`addr2line --exe={{可执行文件地址}} --functions --demangle {{地址}}`
