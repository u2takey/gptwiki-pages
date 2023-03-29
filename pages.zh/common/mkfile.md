# mkfile 
## chatgpt 
mkfile命令是MacOS和FreeBSD中的一个命令，用于创建一个具有指定大小和内容的文件。

该命令的语法为：

mkfile [-nv] size[b|k|m|g] filename ...

参数说明：

- -n：不真正创建文件，只打印执行的命令。
- -v：详细输出命令执行过程。
- size：指定文件大小，单位可以是b、k、m或g。例如，100b表示100字节，10k表示10千字节，1m表示1兆字节，1g表示1吉字节。
- filename：指定要创建的文件名。可以同时创建多个文件，用空格分隔。

示例：

以下命令将创建一个大小为100兆字节的空文件：

mkfile 100m filename

以下命令将创建一个大小为10兆字节，内容为随机字符的文件：

mkfile -v 10m filename

以下命令将创建两个大小为1兆字节的空文件：

mkfile 1m file1 file2 

## tldr 
 
> 创建一个或多个任意大小的空文件。
> 更多信息：<https://manned.org/mkfile>.

- 创建一个 15 千字节的空文件：

`mkfile -n {{15k}} {{文件名}}`

- 创建给定大小和单位的文件（bytes, KB, MB, GB）：

`mkfile -n {{大小}}{{b|k|m|g}} {{文件名}}`

- 创建两个 4 兆字节的文件：

`mkfile -n {{4m}} {{文件名 1}} {{文件名 2}}`
