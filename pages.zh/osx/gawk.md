# gawk 
## chatgpt 
gawk是GNU Awk的缩写，是一个文本处理工具。gawk支持多种功能，包括文本分析、即插即用模块、正则表达式等。以下是gawk命令的一些常见用法：

1. 执行脚本：gawk -f script.awk file.txt。file.txt是读取的文件名，script.awk是gawk脚本的文件名。
2. 执行一行命令：gawk 'command' file.txt。gawk会执行单引号内的命令。
3. 查找一个特定的行并打印出来：gawk '/keyword/' file.txt。gawk会查找带有“keyword”关键字的行并打印出来。
4. 打印特定列：gawk '{print $1,$3}' file.txt。gawk会打印文件中的第一列和第三列。
5. 计算文件中所有数字的总和：gawk '{sum += $1} END {print sum}' file.txt。gawk会将文件中的所有数字加起来并打印结果。
6. 使用gawk内置函数：例如，gawk的substr函数可以截取一个字符串的一部分。gawk '{print substr($1,1,3)}' file.txt会打印每一行第一列的前三个字符。

这些只是gawk的一些用法示例，gawk可执行的操作和函数非常多，非常适合用来对文本数据进行处理和分析。 

## tldr 
 
> 这是 `-p linux awk` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux awk`
