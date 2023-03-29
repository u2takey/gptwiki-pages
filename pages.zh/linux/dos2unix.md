# dos2unix 
## chatgpt 
dos2unix是一个在Linux操作系统中用于转换文本文件格式的命令。它的作用是将DOS风格的文本文件格式转换为Unix风格的文本文件格式。

在DOS环境下，文本文件中的换行符是CR（回车符）和LF（换行符）两个字符，表示为“\r\n”，而在Unix环境下，文本文件中的换行符仅为LF（换行符）一个字符，表示为“\n”。

dos2unix命令可以将DOS风格的文本文件中的"\r\n"替换为Unix风格的"\n"，从而使得该文本文件可以在Unix/Linux系统中正常使用。

使用dos2unix命令的格式为：

dos2unix [options] [file]

其中，options是一些参数选项，file则是需要转换的文件名。

dos2unix命令的一些常用参数选项包括：

- -k：保留文件的日期和时间戳信息。
- -n：禁止dos2unix将文件转换为Unix格式，保留文件原有的格式。
- -q：静默模式，不输出任何信息。
- -V：显示dos2unix命令的版本信息。
- -help或--help：显示dos2unix命令的帮助信息。

总的来说，dos2unix命令的作用是将DOS风格的文本文件转换为Unix风格的文本文件，使得文本文件可以在Unix/Linux系统中正常使用。 

## tldr 
 
> 将 DOS 样式的行尾更改为 Unix 样式。
> 用 LF 替换 CRLF.
> 更多信息：<https://manned.org/dos2unix>.

- 更改文件的行尾：

`dos2unix {{文件名}}`

- 使用 Unix 样式的行尾创建副本：

`dos2unix -n {{文件名}} {{文件名}}`
