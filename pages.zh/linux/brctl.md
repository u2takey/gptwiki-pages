# brctl 
## chatgpt 
"brctl" 是 Linux 中的一个命令，用于管理 Linux 桥接设备，这是将物理网络设备和虚拟网络设备相连的方式。

使用 "brctl" 可以创建和管理 Linux 桥接设备，包括添加和删除桥接接口、查看桥接信息和状态等。常用命令有：

1. brctl addbr bridge：创建一个新的桥接设备。

2. brctl addif bridge interface：将一个物理网络设备或虚拟网络设备添加到指定的桥接设备中。

3. brctl delbr bridge：删除指定的桥接设备。

4. brctl delif bridge interface：从指定的桥接设备中删除指定的物理网络设备或虚拟网络设备。

5. brctl show：显示当前系统上所有桥接设备的信息。

6. brctl showmacs bridge：显示指定桥接设备中所有连接到它上面的 MAC 地址。

7. brctl stp bridge on/off：开启或关闭指定桥接设备的 Spanning Tree 协议。

总的来说，"brctl" 命令能够有效地管理和配置 Linux 系统中的桥接设备，使得物理设备和虚拟设备能够相互通信、共享数据。 

## tldr 
 
> 以太网桥管理。
> 更多信息：<https://manned.org/brctl>.

- 显示有关当前现有以太网网桥信息的列表：

`sudo brctl show`

- 创建新的以太网桥接接口：

`sudo brctl add {{网桥名}}`

- 删除一个已存在的以太网桥接接口：

`sudo brctl del {{网桥名}}`

- 向现有网桥添加接口：

`sudo brctl addif {{网桥名}} {{接口名}}`

- 从现有网桥中删除接口：

`sudo brctl delif {{网桥名}} {{接口名}}`
