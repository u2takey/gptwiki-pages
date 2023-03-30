# fsck 
## chatgpt 
fsck是一个用于检查和修复Linux文件系统的命令。它的全称是Filesystem Consistency Check，意为文件系统一致性检查。

在Linux系统中，当文件系统出现错误时，fsck能够对其进行检查和修复。它会扫描整个文件系统以查找文件系统中的错误，并尝试修复这些错误。这些错误可能是由突然的系统故障、硬件故障、系统崩溃、停电等原因引起的。

fsck的使用需要root权限，因为它需要对文件系统进行读写操作。它可以检查ext2、ext3、ext4、FAT、NTFS等各种类型的文件系统。

一般情况下，使用fsck时，应先卸载文件系统，以确保文件系统不受其他进程的干扰。如果文件系统无法卸载，则需要在修复过程中使用只读模式，这将使fsck仅报告错误，而不进行任何修复。

基本语法：

```
fsck [选项] 文件系统
```

常用选项：

- -a：自动修复文件系统中的错误；
- -n：不要对文件系统进行修复和修改，仅报告错误；
- -r：自动修复文件系统中的错误，并在修复过程中忽略用户输入的所有提示。

注意：使用fsck时需要谨慎，因为它可能会删除或破坏文件系统中的数据，特别是在进行强制修复时。因此，在使用fsck之前，请务必备份您的数据。 

## tldr 
 
> 检查或修复文件系统的完整性，运行命令时应卸载文件系统。
> 它是一个包装器，包含 `fsck_hfs`, `fsck_apfs`, `fsck_msdos`, `fsck_exfat`, `fsck_udf` 作为可选。
> 更多信息：<https://ss64.com/osx/fsck.html>.

- 检查文件系统 /dev/sda，报告损坏的块：

`fsck {{/dev/sda}}`

- 仅当文件系统 /dev/sda 是干净的时才检查它，报告任何损坏的块并以交互方式让用户选择修复每个块：

`fsck -f {{/dev/sda}}`

- 仅当文件系统 /dev/sda 干净时才检查它，报告任何损坏的块并自动修复它们：

`fsck -fy {{/dev/sda}}`

- 检查文件系统 /dev/sda, 报告是否已完全卸载：

`fsck -q {{/dev/sda}}`