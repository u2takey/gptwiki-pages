# gshred 
## chatgpt 
gshred是一个命令行工具，用于安全地删除文件和目录中的数据。它使用安全的数据销毁算法来重复覆盖数据，以确保它无法恢复。

命令语法如下：

gshred [OPTIONS] FILE

其中OPTIONS包括：

-v, --verbose：显示删除进度

-z, --zero：在最后一次覆盖后用零填充

--iterations=N：指定覆盖数据的次数，默认为3

--size=N：指定每次覆盖的数据块大小，默认为1MiB

--remove：删除FILE后再清空

--help：显示帮助信息

--version：显示版本信息

例如，要以默认设置使用gshred删除文件file.txt，可以在终端中键入：

gshred file.txt

要以最大覆盖数据次数和覆盖数据块大小为10和2MiB删除目录dir，可以键入：

gshred --iterations=10 --size=2MiB -rv dir/ 

## tldr 
 
> 这是 `-p linux shred` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux shred`
