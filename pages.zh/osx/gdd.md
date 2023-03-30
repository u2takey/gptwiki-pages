# gdd 
## chatgpt 
命令：gdd

gdd是GNU dd的一个变种，它是一个用于复制和转换文件的命令行工具。与标准dd命令不同，gdd还支持多种输入输出格式，包括二进制格式、ASCII格式、EBCDIC格式、IBM S390格式等。

命令格式:

gdd [ 安装选项 ] [ 是否阻塞 ] [ 字节数目 ] [ 来源 ] [ 目标 ]

命令参数:

安装选项：这些选项包括 noerror、notrunc、sync、fsync 等。

noerror：gdd 复制时遇到错误，不立刻退出。

notrunc：不截断输出文件。

sync：一次写入操作成功后，强制刷到硬盘上。

fsync：每次写入后刷到硬盘上。

是否阻塞：to=和from=之间设置同步和异步选项，可以使用字母序列“succeeds”，“failed”等。

字节数目：可以设置每次读写的字节数目，可以使用经过优化的计算方法。

源：输入文件名。

目标：输出文件名。

命令功能：

gdd命令用于将一个文件的内容复制到另一个文件中，也可以用于复制磁盘镜像文件到物理设备、制作引导盘等。使用gdd命令时，需要指定源文件和目标文件，以及适当的命令选项。

命令示例：

1. 将源文件复制到目标文件：

  gdd if=inputfile of=outputfile

2. 创建1KB大小的文件：

  gdd if=/dev/zero of=outputfile bs=1024 count=1

  这个命令将创造一个大小为1KB的文件。

3. 将ISO镜像文件写入USB设备：

  gdd if=ubuntu-18.04-desktop-amd64.iso of=/dev/sdb bs=4M status=progress

  这个命令将ISO镜像文件写入USB设备/dev/sdb中，并指定了一个块大小为4MB的缓冲区，并进行了传输的进度情况的输出。

注意：

gdd命令是Linux系统中一个十分重要的工具，但因为其强大的操作性和易导致数据丢失的风险，请谨慎使用。在使用gdd命令时，一定要确认文件名、磁盘设备名、选项设置等。如果操作有误，可能导致数据被覆盖或丢失。 

## tldr 
 
> 这是 `-p linux dd` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux dd`
