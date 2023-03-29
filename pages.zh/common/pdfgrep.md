# pdfgrep 
## chatgpt 
pdfgrep是一款在PDF文件中搜索文本的命令行工具。它的语法为：

pdfgrep [选项] 搜索词 [文件名]

其中，选项可以用来设置搜索的模式、输出格式、搜索范围等。

常用的选项包括：

- -i：忽略大小写
- -v：反向匹配，即只输出没有匹配的行
- -E：启用正则表达式模式
- -F：禁用正则表达式模式，直接按照搜索词进行匹配
- -c：仅输出匹配行的数量
- -m：仅输出前N个匹配的行
- -A N：在匹配行后输出N行
- -B N：在匹配行前输出N行
- -C N：在匹配行前后各输出N行
- -r：递归搜索子目录中的PDF文件

使用实例：

1. 搜索PDF文件中包含特定词汇的行：

$ pdfgrep -i "apple" example.pdf

2. 搜索指定目录及其子目录中的所有PDF文件：

$ pdfgrep -r "banana" /path/to/directory/

3. 仅输出匹配行的数量：

$ pdfgrep -c "orange" example.pdf

4. 输出匹配行及其上下各2行：

$ pdfgrep -C 2 "grape" example.pdf

总之，pdfgrep是一款非常方便实用的PDF文本搜索工具，可用于在大量PDF文档中快速查找相关内容。 

## tldr 
 
> 在 PDF 文件中搜索文本。
> 更多信息：<https://pdfgrep.org>.

- 在 PDF 中查找与关键词匹配的行：

`pdfgrep {{关键词}} {{文件.pdf}}`

- 包含每个匹配行的文件名和页码：

`pdfgrep --with-filename --page-number {{关键词}} {{文件.pdf}}`

- 对以 "foo" 开头关键词搜索，返回前 3 个匹配项，不区分大小写：

`pdfgrep --max-count {{3}} --ignore-case {{'^foo'}} {{文件.pdf}}`

- 在当前目录中扩展名为.pdf 的文件中递归查找关键词：

`pdfgrep --recursive {{关键词}}`

- 在与当前目录中特定文件名 "*book.pdf" 匹配的文件上递归查找关键词：

`pdfgrep --recursive --include {{'*book.pdf'}} {{关键词}}`
