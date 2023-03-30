# gbasename 
## chatgpt 
命令：gbasename

gbasename命令是Linux中的一种基本命令，用于在给定的路径中获取文件或路径名的基本名称。

语法：gbasename [OPTIONS] NAME [SUFFIX]

参数说明：
- OPTIONS：支持以下选项
  - -a，--multiple：打印多个结果，名称中的每个非空前缀都是给定路径的一个项。
  - -s，--suffix=SUFFIX：从NAME中移除后缀SUFFIX。
  - -z，--zero：用null字符作为分隔符。
- NAME：指定路径名称，可以是文件名或目录名。
- SUFFIX：指定需要从指定名称中删除的后缀。

示例：
1. 获取路径名的基本名称：gbasename /home/user/filename.txt
   输出：filename.txt
2. 移除文件名中的后缀：gbasename /home/user/filename.txt .txt
   输出：filename
3. 打印多个结果：gbasename -a /home/user/filename.txt
   输出：filename.txt filename user home /

备注：
- gbasename命令与basename命令类似，但使用不同的算法来处理文件名和路径名。gbasename使用GNU C库提供的函数，而basename使用系统libc提供的函数。 

## tldr 
 
> 这是 `-p linux basename` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux basename`
