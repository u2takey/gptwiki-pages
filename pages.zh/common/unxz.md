# unxz 
## chatgpt 
unxz是一个解压缩工具，用于解压xz压缩的文件。

具体来说，unxz命令将输入文件中的xz压缩数据解压缩成原始数据，并将结果输出到标准输出或指定的输出文件中。

其基本语法如下：

unxz [选项] 文件名

选项包括：

- -c或--stdout：将解压缩的数据输出到标准输出而不是文件；
- -d或--decompress：与-c选项一起使用，表示只解压缩而不保存输出文件；
- -k或--keep：保留原始的压缩文件；
- -f或--force：强制覆盖输出文件。

例如，执行以下命令可以解压缩名为file.xz的文件：

unxz file.xz

如果要将解压缩的数据输出到标准输出，可以使用-c选项：

unxz -c file.xz

如果要将解压缩的数据输出到标准输出并且不保存输出文件，则可以使用-d选项：

unxz -dc file.xz

如果要强制覆盖输出文件，则可以使用-f选项：

unxz -f file.xz

如果想要保留原始的压缩文件，可以使用-k选项：

unxz -k file.xz 

## tldr 
 
> 这是 `xz` 命令的一个别名。
> 更多信息：<https://manned.org/unxz>.

- 原命令的文档在：

`tldr xz`
