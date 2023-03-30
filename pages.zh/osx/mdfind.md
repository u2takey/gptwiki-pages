# mdfind 
## chatgpt 
mdfind命令是macOS中的一个命令行工具，用于在本地磁盘上搜索指定的文件、文件夹或内容。mdfind使用Spotlight搜索技术来查找文件，支持使用各种条件、关键字和过滤器来缩小搜索范围。

以下是mdfind命令的语法和参数：

语法：mdfind [options] query

参数：
- name：按文件名搜索
- kind：按文件类型搜索
- size：按文件大小搜索
- mtime：按修改时间搜索
- kMDItemAuthor：按作者搜索
- kMDItemCopyright：按版权信息搜索
- kMDItemContentType：按文件内容类型搜索

举例说明：
1. mdfind -name "file.txt" : 搜索本地磁盘上所有名为“file.txt”的文件。
2. mdfind -kind "PDF" : 查找所有PDF文件。
3. mdfind -size +500M : 查找大于500MB的文件。
4. mdfind -mtime -1w : 查找最近一周内被修改过的文件。
5. mdfind -onlyin ~/Documents/ -name "*.pdf" : 在“文档”文件夹中搜索所有PDF文件。

mdfind命令可以帮助用户快速搜索和定位本地磁盘上的文件和内容。它适用于需要在大量文件中查找特定信息的情况，例如查找特定文件类型、文件名、作者、大小和修改时间等。 

## tldr 
 
> 列出与给定查询匹配的文件。
> 更多信息：<https://ss64.com/osx/mdfind.html>.

- 按文件名查找文件：

`mdfind -name {{文件}}`

- 按内容查找文件：

`mdfind {{查找的字符串}}`

- 在给定目录中查找包含字符串的文件：

`mdfind -onlyin {{目录}} {{字符串}}`
