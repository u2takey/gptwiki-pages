# glocate 
## chatgpt 
命令 glocate 是 GNU Locate 的前端。 GNU Locate 是一个全文本搜索工具，可快速查找计算机中的文件和目录。 与普通的文件搜索工具不同，glocate 不像其他文件搜索工具那样扫描磁盘，而是使用一个数据库，该数据库通过定期扫描计算机来维护，以获取文件和目录的位置，包括它们的元数据（例如，大小、修改日期等）。通过这种方式，glocate 能够提供更快的搜索速度，尤其是搜索大型文件系统时。一些常用的选项包括：

- -i：忽略大小写
- -l：限制输出数量
- -r：正则表达式搜索
- -w：按单词搜索
- -c：输出文件计数而不是文件名
- -H：不要显示文件名

以下是一些示例用法：

- 搜索包含特定字符串的所有文件：glocate string
- 搜索具有特定扩展名的文件：glocate '*.txt'
- 搜索文件名匹配正则表达式的文件：glocate -r pattern
- 查找特定用户拥有的文件：glocate -U username
- 查找在给定时间之后修改的文件：glocate -m time_string

请注意，使用 glocate 命令需要提前安装 GNU Locate 工具和创建 Locate 数据库。GNU Locate 的数据库可以使用命令 updatedb 更新。例如：sudo updatedb 。 

## tldr 
 
> 这是 `-p linux locate` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux locate`
