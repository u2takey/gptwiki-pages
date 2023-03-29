# sccmap 
## chatgpt 
sccmap是一个在Solaris操作系统中使用的命令，用于查看和管理SCSI控制器映射表。SCSI是一种通用的接口协议，用于在计算机和外部设备之间传输数据。SCSI控制器映射表是一个包含SCSI控制器及其相关设备的列表，这些设备可能是硬盘、磁带机、CD-ROM、DVD、打印机等。

sccmap命令的用法是：sccmap [-D device] [-I] [-s] [-m map] [controller | device]

-D：指定要查询的SCSI设备。默认情况下，sccmap将使用标准的/dev/scsi设备。可以指定特定的SCSI设备，例如/dev/rdsk/c0t3d0s0。

-I：显示SCSI总线信息。

-s：仅显示SCSI控制器的名称和设备的符号链接。

-m：指定要查询的SCSI控制器映射表文件。默认情况下，sccmap将使用/etc/scsi/sdevice.conf文件。

controller：指定SCSI控制器的名称，例如c0或c1。

device：指定SCSI设备的设备文件名，例如/dev/rdsk/c0t3d0s0。

通常情况下，sccmap命令用于查看SCSI控制器映射表，以便检查设备是否正确配置。 它还可用于管理SCSI控制器映射表，例如添加或删除设备。 

## tldr 
 
> 提取有向图的强连通分量。
> Graphviz 过滤器：`acyclic`、`bcomps`、`comps`、`edgepaint`、`gvcolor`、`gvpack`、`mingle`、`nop`、`sccmap`、`tred` 和 `unflatten`。
> 更多信息： <https://www.graphviz.org/pdf/sccmap.1.pdf>.

- 从一个或多个有向图中提取强连通分量：

`sccmap -S {{路径/到/输入1.gv}} {{路径/到/输入2.gv ...}} > {{路径/到/输出.gv}}`

- 打印一个图形的统计信息，不生成输出图形：

`sccmap -v -s {{路径/到/输入1.gv}} {{路径/到/输入2.gv ...}}`

- 显示 `sccmap` 的帮助信息：

`sccmap -?`
