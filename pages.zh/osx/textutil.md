# textutil 
## chatgpt 
textutil是一个在macOS上可用的命令行工具，可以用于方便地转换和处理多种文本格式。以下是textutil的一些常见用法和相关参数：

1. 转换文件格式

可以使用textutil将一个文件从一种文本格式转换为另一种文本格式。例如：

将Word文档转换为纯文本格式：

textutil -convert txt file.doc

将HTML文件转换为富文本格式：

textutil -convert rtf file.html

将富文本格式转换为Word文档：

textutil -convert docx file.rtf

2. 调整文本格式

textutil还可以用于调整文本格式，例如：

将纯文本格式转换为富文本格式：

textutil -convert rtf file.txt

将富文本格式转换为HTML格式：

textutil -convert html file.rtf

3. 合并文本文件

textutil可以将多个文本文件合并成一个文件，例如：

将多个富文本格式文件合并成一个文件：

textutil -cat rtf file1.rtf file2.rtf file3.rtf -output combined.rtf

合并多个HTML文件：

textutil -cat html file1.html file2.html file3.html -output combined.html

总之，textutil是一个非常强大且灵活的文本处理工具，可以大大提高处理文本文件的效率。 

## tldr 
 
> 用于操作各种格式的文本文件。
> 更多信息：<https://ss64.com/osx/textutil.html>.

- 显示有关 `foo.rtf` 的信息：

`textutil -info {{foo.rtf}}`

- 将 `foo.rtf` 转换为 `foo.html`：

`textutil -convert {{html}} {{foo.rtf}}`

- 将带格式的 rtf 文本转换为普通 txt 文本：

`textutil {{foo.rtf}} -convert {{txt}}`

- 将 `foo.txt` 转换为 `foo.rtf`, 字体使用 Times 字号 10：

`textutil -convert {{rtf}} -font {{Times}} -fontsize {{10}} {{foo.txt}}`

- 加载当前目录中的所有 RTF 文件，连接其内容，并将结果作为 `index.html` 写入，HTML 标题设置为"多个文件"：

`textutil -cat {{html}} -title "多个文件" -output {{index.html}} *.rtf`
