# unix2dos 
## chatgpt 
Linux 命令 `unix2dos` 用于将 Unix 文本文件转换为 DOS 文本文件格式。在 Unix 系统中，每一行文本通常以换行符“\n”结束，在 DOS 系统中，每一行文本则以回车符和换行符“\r\n”结束。使用 `unix2dos` 命令可以将 Unix 格式的文本文件转换为 DOS 格式，使得 DOS 系统能够正确地读取该文件。

`unix2dos` 命令的语法如下：

```
unix2dos [options] file1 file2 file3 ...
```

该命令可以接受多个参数，每个参数对应一个需要转换格式的文件。`unix2dos` 命令还支持以下选项：

- `-c`：在转换完每个文件后输出转换结果；
- `-k`：保留原文件的时间戳；
- `-n`：不应用换行符转换；
- `-q`：安静模式，不输出任何信息；
- `-u`：在转换完每个文件后删除原文件。

例如，要将名为 `example.txt` 的文本文件转换为 DOS 格式，可以使用以下命令：

```
unix2dos example.txt
```

转换完成后，原始的 `example.txt` 文件将被替换为 DOS 格式的文件。 

## tldr 
 
> 将 Unix 样式的行尾更改为 DOS 样式。
> 用 CRLF 替换 LF.
> 更多信息：<https://waterlan.home.xs4all.nl/dos2unix.html>.

- 更改文件的行尾：

`unix2dos {{文件名}}`

- 使用 DOS 样式的行尾创建副本：

`unix2dos -n {{文件名}} {{新文件名}}`
