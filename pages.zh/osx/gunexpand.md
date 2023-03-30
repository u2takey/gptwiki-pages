# gunexpand 
## chatgpt 
gunexpand是一个Linux命令，用于将gzip压缩格式的文件进行解压缩。它是gzip工具包的一部分。

详细的解释如下：

语法：

```gunexpand file.gz```

参数说明：

```file.gz```：指定需要解压缩的gzip压缩格式的文件名。

gunexpand命令解压缩gzip文件并将其转换为二进制文件。

gzip是一种常见的文件压缩格式，通常用于压缩大文件，以节约磁盘空间，并在传输文件时加快速度。gunexpand是gzip工具包的一部分，它可将gzip压缩的文件解压缩成原始文件。

使用gunexpand命令时，您需要指定需要解压缩的gzip文件的名称。该命令将读取gzip文件中的数据，并将其解压缩到一个新的二进制文件中。解压缩后的文件将与原始文件具有相同的名称（减去.gz扩展名），但不再是gzip压缩格式。

gunexpand命令还具有其他选项，例如可以在stdin中指定gzip格式的数据。具体细节请参阅gunexpand命令的手册页。 

## tldr 
 
> 这是 `-p linux unexpand` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux unexpand`
