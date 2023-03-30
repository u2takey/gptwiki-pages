# diskutil 
## chatgpt 
diskutil是用于管理磁盘的命令行实用程序，它可以在Mac OS X和macOS操作系统中管理本地和本地连接的存储设备。它可以对存储设备进行多种操作，如创建新的分区、格式化磁盘、挂载和卸载卷、修复损坏的磁盘、检查磁盘状态、克隆卷等。

以下是diskutil的一些常用选项和子命令：

选项：
- list：列出所有磁盘和卷
- info：显示磁盘或卷的信息
- verifyDisk：验证磁盘是否有错误
- repairDisk：修复错误的磁盘
- eraseDisk：擦除磁盘并用指定的格式重新格式化
- mount：挂载指定卷
- unmount：卸载指定卷或设备
- rename：重命名卷或设备
- resizeVolume：调整卷大小
- mergePartitions：合并相邻的分区

子命令：
- apfs：管理APFS分区和容器
- coreStorage：管理Core Storage分区
- raid：管理RAID阵列
- partitionDisk：分区磁盘
- secureErase：安全地擦除磁盘
- cs：管理Core Storage分区

具体命令及其选项可以通过diskutil --help获取帮助。 

## tldr 
 
> 用于管理本地磁盘和卷的实用程序。
> 更多信息：<https://ss64.com/osx/diskutil.html>.

- 列出所有当前可用的磁盘、分区和已装入的卷：

`diskutil list`

- 修复卷的文件系统数据结构：

`diskutil repairVolume {{目标卷文件}}`

- 卸载卷：

`diskutil unmountDisk {{目标卷文件}}`

- 弹出 CD/DVD（先卸载）：

`diskutil eject {{/dev/ 光驱文件名}}`
