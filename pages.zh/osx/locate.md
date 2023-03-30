# locate 
## chatgpt 
命令 `locate` 用于在整个文件系统中查找文件名。它的工作原理是在系统的数据库中搜索文件名，并返回匹配的结果。

数据库是由 `updatedb` 命令创建的。每当 `updatedb` 命令运行时，它会搜索文件系统中的文件并将文件名和其路径存储到一个数据库中。这样，每当你使用 `locate` 命令搜索文件时，它只是在数据库中查找，而不是在整个文件系统中搜索，因此速度非常快。

`locate` 命令支持参数来进一步限制搜索范围、指定文件类型、使用正则表达式检索等功能，例如：

- `locate filename`：查找文件名中包含 “filename” 字符串的所有文件。
- `locate -b filename`：查找完全匹配文件名 “filename” 的文件。
- `locate -i filename`：在搜索时忽略大小写。
- `locate -r 'filename.*txt$'`：使用正则表达式将所有以 “filename” 开头并以 “txt” 结尾的文件名匹配。
- `locate -e filename`：只查找存在的文件。
- `locate -L path`：扩展搜索到指定目录的符号链接。

需要注意的是，由于 `locate` 命令基于数据库，因此它可能会显示不是最新的文件位置。在使用 `locate` 命令之前，建议先运行 `updatedb` 命令更新数据库。 

## tldr 
 
> 快速查找文件名。
> 更多信息：<https://manned.org/locate>.

- 在数据库中查找关键字。注意：数据库定期重新更新（通常每周或每天）：

`locate {{关键字}}`

- 按文件名查找文件（不包含填充字符的模式被解释为 `*关键字*`）：

`locate */{{文件名}}`

- 重新建立文件数据索引数据库。如果要查找最近添加的文件，则需要执行此操作：

`sudo /usr/libexec/locate.updatedb`
