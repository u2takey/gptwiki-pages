# grealpath 
## chatgpt 
命令：grealpath

grealpath 命令用于查找给定路径的绝对路径。它与 realpath 命令类似，但是它在不同的操作系统上均可用，并支持多个平台特定选项。

语法：

grealpath [OPTION]... FILENAME...

选项：

-a, --all

打印文件的所有绝对路径，而不是只输出第一个绝对路径。

-m, --no-symlink-components

如果路径包含符号链接，那么输出结果不包括符号链接相关的文件夹组件。

-p, --physical

表示不跟随符号链接，而是输出符号链接的物理路径。

-r, --relative-to=DIR

输出相对于 DIR 参数的路径。

-z, --null

使用类似于 find 命令的 null 分隔符，而不是像默认情况下那样在每行末尾添加换行符。

-V, --version

打印版本号并退出。

-h, --help

显示帮助信息并退出。

用法示例：

1. 打印文件的绝对路径：

grealpath myfile.txt

2. 打印文件的所有绝对路径：

grealpath -a myfile.txt

3. 输出符号链接的物理路径：

grealpath -p symlink_filename

4. 输出路径相对于指定目录的路径：

grealpath -r /home/myDir /home/myDir/myfile.txt

5. 使用 null 分隔符输出结果：

grealpath -z myfile.txt

总结：

grealpath 命令与 realpath 命令类似，但它支持多个平台特定选项，可以在不同的操作系统上使用。它可以用来查找文件的绝对路径，并支持不同的选项来输出符号链接的物理路径，以及相对于指定目录的路径等。 

## tldr 
 
> 这是 `-p linux realpath` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux realpath`
