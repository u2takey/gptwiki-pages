# gfind 
## chatgpt 
"gfind" 不是标准的 Linux 命令，可能是某些 Linux 发行版或软件包中的工具。如果是指 "find" 命令，它是一个用于在 Linux 文件系统中搜索文件的命令。

"find" 命令有一些常用选项：

- `-name`: 按照文件名搜索，支持通配符。
- `-type`: 按照文件类型搜索，如 "f" 表示普通文件，"d" 表示目录。
- `-mtime`: 按照修改日期搜索，+N 表示 N 天前，-N 表示 N 天内，0 表示今天。
- `-size`: 按照文件大小搜索，支持一些单位如 "k" 表示 KB。
- `-exec`: 对搜索到的文件执行指定的命令，必须以 "; \\" 结尾。
- `-print`: 输出搜索到的文件路径，默认行为。

使用示例：

  $ find /path/to/search -name "*.txt" -type f -mtime +7 -print
  $ find /path/to/search -size +10M -exec rm {} \; 

## tldr 
 
> 这是 `-p linux find` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux find`
