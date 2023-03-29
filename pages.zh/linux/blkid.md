# blkid 
## chatgpt 
blkid 命令用于显示指定设备的文件系统类型和UUID等信息。

该命令会读取指定设备的超级块信息来确定设备的文件系统类型，然后输出该设备的唯一标识符，如UUID、LABEL等信息。

使用 blkid 命令可以方便地查看磁盘、分区等设备的一些必要信息，例如文件系统类型、UUID、LABEL等，这些信息在配置系统、挂载设备等场景下非常有用。 

## tldr 
 
> 列出所有已识别的分区及其通用唯一标识符 (UUID)。
> 更多信息：<https://manned.org/blkid>.

- 列出所有分区：

`sudo blkid`

- 列出表中的所有分区，包括当前挂载点：

`sudo blkid -o list`
