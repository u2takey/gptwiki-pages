# file 
## chatgpt 
file命令是一个Linux和Unix操作系统的命令，用于确定文件的类型。它用于快速检查文件的类型，包括文本文件，二进制文件，数据文件等。

命令用法:

file [OPTION]... [FILE]...

参数:

- -b或--brief：列出文件类型时不显示文件名称。
- -c或--checking-printout：类似-v参数，但是对据库文件不影响。
- -f<名称文件>或--file=<名称文件>：从指定的<名称文件>中读取要检查文件的文件名列表。
- -F<分隔符>或--separator=<分隔符>：在文件名列表中，用指定的<分隔符>代替换行符”\n”。
- -h：显示帮助信息并退出。
- -i或--mime：以MIME方式输出文件类型。
- -I或--mime-encoding：以MIME方式输出文件类型（不包括文件名称）。
- -l或--list：列出所有已识别的文件类型。
- -m或--magic-file<文件>：指定一个不同的魔法文件路径。
- -n或--no-buffer：禁用I / O缓冲区。
- -p或--preserve-date：保持源文件的访问时间戳。
- -s或--special-files：轮流测试特殊文件，如字符设备和套接字。
- -v或--verbose：详细输出，包括扩展信息。
- -z或--uncompress：对每个压缩的文件执行解压缩操作。

示例:

1. 检测文件类型

file example.txt

输出结果为：example.txt: ASCII text

2. 检测多个文件类型

file example1.txt example2.pdf

输出结果为：

example1.txt: ASCII text
example2.pdf: PDF document, version 1.5

3. 使用 -b 参数输出文件类型

file -b example.txt

输出结果为：ASCII text

4. 使用 -i 参数以MIME方式输出文件类型

file -i example.txt

输出结果为：text/plain

5. 列出所有已知的文件类型及其对应的描述

file -l

输出结果为：

accounting:             ASCII text
adjtime:                empty
aegis:                  ASCII text
aif:                    Apple/SGI AIFF audio
aiff:                   Apple/SGI AIFF audio
alsa:                   ASCII text
amiga:                  ASCII text
apache:                 ASCII text, with CRLF line terminators

6. 指定要检查的文件列表

file -f filelist.txt

该命令会从filelist.txt文件中读取要检查的文件列表，并输出它们的文件类型。 

## tldr 
 
> 确定文件类型。
> 更多信息：<https://manned.org/file>.

- 提供指定文件类型的描述，对于没有文件扩展名的文件可以正常工作：

`file {{文件名}}`

- 查看压缩文件并确定其中的文件类型：

`file -z {{xxx.zip}}`

- 允许文件与特殊文件或设备文件一起使用：

`file -s {{文件名}}`

- 不要在第一个文件类型匹配时停止；继续执行直到文件结束：

`file -k {{文件名}}`

- 确定文件的 MIME 编码类型：

`file -I {{文件名}}`
