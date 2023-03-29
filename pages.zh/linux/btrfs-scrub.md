# btrfs scrub 
## chatgpt 
btrfs scrub是一种Linux命令，用于在Btrfs文件系统上执行数据完整性检查。Btrfs是一种类似于ZFS的高级文件系统，它包括了许多强大的数据管理功能，例如快照、克隆、数据压缩和RAID数据保护。

在Btrfs文件系统上执行scrub命令可以检查文件系统中的数据，找出可能已经损坏或损坏的数据块。这种检查对于数据丢失或损坏的情况非常有用，因为文件系统可以自动修复发现的损坏。在数据损坏的情况下，scrub命令可以帮助更早地发现问题并更快地解决它。

命令语法如下：
btrfs scrub [options] [filesystem...]

选项与参数说明如下：

- -B：使用一致性检查。
- -c：使用“no-cow”cow操作和被修改过的chunk（遍历整个文件系统，这可能需要较长时间）。
- -d：对文件系统中所有的数据和元数据块执行scrub操作。
- -D：禁用自动校验和修复损坏的数据块。
- -f：即使磁盘不是清洁的也强制执行scrub操作。
- -m：检查元数据块。
- -p N：检查时会报告进度，每N个chunk将会报告一次。

需要注意的是，scrub命令可能需要较长的时间来执行，具体取决于系统的大小和复杂性。建议在周期性地执行scrub命令以确保文件系统完整性。 

## tldr 
 
> 清理 btrfs 文件系统以验证数据完整性。
> 建议每月运行一次 scrub.
> 更多信息：<https://btrfs.readthedocs.io/en/latest/btrfs-scrub.html>.

- 开始 scrub：

`sudo btrfs scrub start {{指向挂载点的路径}}`

- 显示正在进行或上次完成的 scrub 的状态：

`sudo btrfs scrub status {{指向挂载点的路径}}`

- 取消正在进行的 scrub：

`sudo btrfs scrub cancel {{指向挂载点的路径}}`

- 恢复先前取消的 scrub：

`sudo btrfs scrub resume {{指向挂载点的路径}}`

- 开始擦洗，但要等到 scrub 完成后才能退出：

`sudo btrfs scrub start -B {{指向挂载点的路径}}`

- 在安静模式下启动 scrub（不打印错误或统计信息）：

`sudo btrfs scrub start -q {{指向挂载点的路径}}`
