# find 
## chatgpt 
find命令是一个用于在文件系统中查找文件和目录的命令。它可以搜索指定目录及其所有子目录下符合条件的文件，并且可以对搜索结果进行不同的操作。

find命令的语法为：

```
find path expression
```

其中，path表示要搜索的目录路径，expression用于指定搜索条件。

find命令的常用选项包括：

- -name：根据文件名搜索；
- -type：根据文件类型搜索；
- -mtime：根据文件修改时间搜索；
- -size：根据文件大小搜索；
- -exec：对搜索结果执行指定命令。

示例：

- 搜索目录下所有以.txt结尾的文件：`find /path/to/dir -name "*.txt"`
- 搜索目录下所有文件类型为目录的项：`find /path/to/dir -type d`
- 搜索目录下所有最近一天内修改过的文件：`find /path/to/dir -mtime -1`
- 搜索目录下所有文件大小大于1MB的文件：`find /path/to/dir -size +1M`
- 对搜索结果执行指定命令：`find /path/to/dir -name "*.txt" -exec rm {} \;` （删除所有以.txt 结尾的文件） 

## tldr 
 
> 在指定目录树下递归查找文件或目录。
> 更多信息：<https://manned.org/find>.

- 通过扩展名查找文件：

`find {{指定目录}} -name '{{*.ext}}'`

- 查找匹配多个路径或名称模式的文件：

`find {{指定目录}} -path '{{**/path/**/*.ext}}' -or -name '{{*pattern*}}'`

- 查找匹配指定名称的目录，不区分大小写：

`find {{指定目录}} -type d -iname '{{*lib*}}'`

- 查找匹配指定模式的文件，排除特定路径：

`find {{指定目录}} -name '{{*.py}}' -not -path '{{*/site-packages/*}}'`

- 查找符合指定大小范围的文件：

`find {{指定目录}} -size {{+500k}} -size {{-10M}}`

- 对每个文件运行命令（在命令中使用 `{}` 代表当前文件）：

`find {{指定目录}} -name '{{*.ext}}' -exec {{wc -l {} }}\;`

- 查找最近 7 天修改的文件并删除：

`find {{指定目录}} -daystart -mtime -{{7}} -delete`

- 查找空（0 字节）的文件并删除：

`find {{指定目录}} -type {{f}} -empty -delete`
