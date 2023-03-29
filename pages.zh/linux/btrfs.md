# btrfs 
## chatgpt 
btrfs是一种先进的文件系统，是Linux中的一种文件系统类型，也可以作为Linux中磁盘分区的一种选项。它提供了高效的数据管理和存储，支持快照、压缩、数据校验等诸多功能。

btrfs命令是用于管理btrfs文件系统的命令，主要包括以下常用选项：

1. btrfs device：管理btrfs文件系统中的设备。

2. btrfs subvolume：管理btrfs文件系统中的子卷，可创建、删除、重命名、挂载和卸载子卷。

3. btrfs balance：用于平衡btrfs文件系统中的数据和元数据的分布，以提高文件系统的性能和可用性。

4. btrfs scrub：用于对btrfs文件系统中的数据进行校验，并修复任何出现的问题。

5. btrfs snapshot：创建btrfs文件系统中的快照，以便备份、回滚和测试文件系统状态。

6. btrfs send/receive：用于将btrfs文件系统中的子卷或快照推送到另一个计算机，以备份或迁移文件系统。

总之，btrfs命令是一种强大的工具，它可以用于管理高效的文件系统，并提供了丰富的功能来保护和管理数据。 

## tldr 
 
> 一种基于写时复制（COW）原理的 Linux 文件系统。
> 此命令也有关于其子命令的文件，例如：`btrfs device`.
> 更多信息：<https://btrfs.readthedocs.io/en/latest/btrfs.html>.

- 创建子卷：

`sudo btrfs subvolume create {{指向子卷的路径}}`

- 列出子卷：

`sudo btrfs subvolume list {{指向挂载点的路径}}`

- 显示空间使用情况信息：

`sudo btrfs filesystem df {{指向挂载点的路径}}`

- 启用配额（quota）：

`sudo btrfs quota enable {{指向子卷的路径}}`

- 显示配额（quota）：

`sudo btrfs qgroup show {{指向子卷的路径}}`
