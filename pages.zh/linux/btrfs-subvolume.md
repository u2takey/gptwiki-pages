# btrfs subvolume 
## chatgpt 
简介：
btrfs 是一种先进的文件系统，支持诸如磁盘损坏检测、快照、压缩和子卷等高级功能。子卷是 btrfs 的一个重要特性，可以帮助用户对数据进行管理和组织。

btrfs subvolume 命令是用于创建、删除、修改和浏览子卷的工具。

具体解释：
1. 创建子卷：
使用 btrfs subvolume create 命令可以在文件系统上创建一个新的子卷。例如，要在 /mnt/btrfs 目录下创建一个名为 mysubvol 的子卷，可以使用以下命令：

```
btrfs subvolume create /mnt/btrfs/mysubvol
```

2. 删除子卷：
使用 btrfs subvolume delete 命令可以删除一个已存在的子卷。例如，要删除之前创建的 mysubvol 子卷，可以使用以下命令：

```
btrfs subvolume delete /mnt/btrfs/mysubvol
```

请注意，删除子卷不会删除子卷中的数据。如果要删除子卷和数据，请使用 btrfs subvolume delete --recursive 命令。

3. 修改子卷：
使用 btrfs subvolume snapshot 命令可以创建子卷的快照。快照是子卷数据的只读副本。例如，要为 mysubvol 子卷创建一个名为 mysnap 的快照，可以使用以下命令：

```
btrfs subvolume snapshot /mnt/btrfs/mysubvol /mnt/btrfs/mysnap
```

可以使用 btrfs subvolume snapshot -r 命令创建读写快照。

4. 浏览子卷：
使用 btrfs subvolume list 命令可以列出文件系统上的所有子卷。例如，要列出 /mnt/btrfs 目录下的所有子卷，可以使用以下命令：

```
btrfs subvolume list /mnt/btrfs
```

此外，btrfs subvolume show 命令可以显示指定子卷的详细信息。

总结：
btrfs subvolume 命令是管理 btrfs 文件系统子卷的一个重要工具，允许用户创建、删除、修改和浏览子卷。使用这些命令可以帮助用户更有效地管理其数据，并保证数据的安全性和可靠性。 

## tldr 
 
> 管理 btrfs 子卷和快照。
> 更多信息：<https://btrfs.readthedocs.io/en/latest/btrfs-subvolume.html>.

- 创建一个新的空子卷：

`sudo btrfs subvolume create {{指向新子卷的路径}}`

- 列出指定文件系统中的所有子卷和快照：

`sudo btrfs subvolume list {{指向 btrfs 文件系统的路径}}`

- 删除一个子卷：

`sudo btrfs subvolume delete {{指向子卷的路径}}`

- 创建现有子卷的只读快照：

`sudo btrfs subvolume snapshot -r {{指向源子卷的路径}} {{指向目标的路径}}`

- 创建现有子卷的读写快照：

`sudo btrfs subvolume snapshot {{指向源子卷的路径}} {{指向目标的路径}}`

- 显示有关子卷的详细信息：

`sudo btrfs subvolume show {{指向子卷的路径}}`
