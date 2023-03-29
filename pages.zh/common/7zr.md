# 7zr 
## chatgpt 
7zr是7-Zip的一个命令行版本，可以在终端或命令提示符下使用。它能解压、压缩和归档文件。

具体命令：

- 7zr x：解压文件。例如：7zr x filename.7z
- 7zr a：压缩文件。例如：7zr a archive.7z /path/to/files/
- 7zr l：列出归档文件中的所有文件和目录。例如：7zr l filename.7z
- 7zr t：测试归档文件的完整性。例如：7zr t filename.7z
- 7zr e：提取文件，但不保留目录结构。例如：7zr e filename.7z

此外，还有一些其他选项可以用于修改压缩级别、设置密码、分卷压缩、过滤文件等。可以使用命令“7zr --help”获取更多信息。 

## tldr 
 
> 一个高压缩率的文件归档器。
> 类似于 `7z`，只支持 `.7z` 文件。
> 更多信息：<https://www.7-zip.org>.

- 归档一个文件或目录：

`7zr a {{归档文件.7z}} {{文件或目录}}`

- 加密一个已存在的归档文件（包括文件名）：

`7zr a {{加密文件.7z}} -p{{密码}} -mhe=on {{归档文件.7z}}`

- 提取一个已存在的 7z 文件，并保持原来的目录结构：

`7zr x {{归档文件.7z}}`

- 提取一个归档文件到指定的输出目录：

`7zr x {{归档文件.7z}} -o{{输出目录}}`

- 提取一个归档文件到标准输出：

`7zr x {{归档文件.7z}} -so`

- 列出一个归档文件的内容：

`7zr l {{归档文件.7z}}`

- 列出可用的归档文件类型：

`7zr i`