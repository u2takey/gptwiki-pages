# hexdump 
## chatgpt 
hexdump是一个在Linux和Unix系统中可用的命令行工具，用于将二进制文件的数据以十六进制和ASCII码的格式进行输出。

它可以用来执行各种操作，如

1. 以视觉化的方式查看文件的内容

2. 分析文件结构

3. 发现文件中的隐藏信息

4. 将数据从二进制格式转换为文本格式

当使用hexdump命令时，可以提供许多选项来控制输出的格式和内容。

以下是常见的选项：

-b：以8位二进制格式输出数据

-c：以字符的ASCII码的方式输出

-d：以有符号整数的十进制格式输出数据

-o：以有符号整数的八进制格式输出数据

-x：以16位十六进制格式输出数据

除此之外，hexdump还可以用来查看内存映像、网络数据包、硬件设备等。它也被广泛用于各种编程任务中，如调试和字节操作等。

总之，hexdump命令是一种有用的工具，可以用来处理二进制数据并发现其中隐藏的信息。 

## tldr 
 
> 一个 ASCII，十进制，十六进制，八进制转换查看工具。
> 更多信息：<https://manned.org/hexdump>.

- 打印文件的十六进制表示形式：

`hexdump {{路径/到/文件}}`

- 以十六进制显示输入偏移量，并在最后两列中显示其 ASCII 表示形式：

`hexdump -C {{路径/到/文件}}`

- 显示文件的十六进制表示，但只解释输入的 N 个字节：

`hexdump -C -n{{字节数}} {{路径/到/文件}}`
