# ripgrep 
## chatgpt 
ripgrep是一款快速、用于在文件内容中搜索字符串的命令行工具。它使用Rust编写，以速度和性能著称，常常被称为其它搜索工具（如grep、ack和ag）的替代品。以下是该命令的一些常用参数和用例：

- `ripgrep pattern`: 在当前目录下查找包含指定字符串“pattern”的文件。
- `ripgrep -i pattern`: 不区分大小写地搜索指定字符串。
- `ripgrep -v pattern`: 反向搜索字符串，即只显示不包含该字符串的行。
- `ripgrep -w pattern`: 只匹配完整的单词，而不是包含该字符串的任何子串。 
- `ripgrep --color pattern`: 高亮显示匹配的字符串。
- `ripgrep -n pattern`: 显示匹配字符串的行号。
- `ripgrep -F pattern`: 按照字符串字面意义进行搜索，而不是使用正则表达式。
- `ripgrep --files-with-matches pattern`: 只显示包含匹配字符串的文件名，而不是显示匹配行。

总之，ripgrep在搜索文件内容时非常快速和高效，对于需要快速查找文本内容的任务非常有用。 

## tldr 
 
> 这是 `rg` 命令的一个别名。

- 原命令的文档在：

`tldr rg`
