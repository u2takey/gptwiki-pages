# ged 
## chatgpt 
ged是一个文本编辑器，常用于Linux/Unix系统中，命令格式如下：

ged [选项] [文件]

选项：

- -b 表示以批处理模式打开
- -d debug_level 表示设置调试级别
- -e 表示以expanding模式打开
- -h 表示显示帮助信息
- -n lineno 表示打开文件并跳至指定行
- -v 表示显示版本信息
- -w 表示使用单词模式打开

文件：

需要编辑的文件名或路径，如果不指定则打开一个新文件。

使用：ged 编辑或创建文本文件

例子：

1. 编辑一个新文件

ged

2. 打开一个已存在的文件example.txt

ged example.txt

3. 打开一个文件并跳至第10行

ged -n 10 example.txt

4. 使用批处理模式打开文件

ged -b example.txt 

## tldr 
 
> 这是 `-p linux ed` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux ed`
