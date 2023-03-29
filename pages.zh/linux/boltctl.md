# boltctl 
## chatgpt 
boltctl是一个Linux命令，它与“Thunderbolt控制器”（或简称为“bolt”）交互。Thunderbolt是一种连接电脑和外部设备的高速接口，类似于USB或HDMI。boltctl命令可用于管理系统上的Thunderbolt设备。

常见的用法包括：

- boltctl list：列出所有已知的Thunderbolt设备。
- boltctl enroll <device>：将Thunderbolt设备添加到授权列表中，以便可以在未来使用它。
- boltctl forget <device>：从授权列表中删除Thunderbolt设备。
- boltctl authorize <device>：授权将来连接到Thunderbolt设备。
- boltctl deauthorize <device>：取消授权以连接到Thunderbolt设备。

这些命令需要root权限才能运行。运行boltctl时，通常会提供有关其他可用命令和选项的详细信息。 

## tldr 
 
> 控制雷电（thunderbolt）设备。
> 更多信息：<https://manned.org/boltctl>.

- 列出已连接并授权的设备：

`boltctl`

- 列出已连接的设备，且包含未授权的设备：

`boltctl list`

- 临时授权一个设备：

`boltctl authorize {{设备uuid}}`

- 授权并记住一个设备：

`boltctl enroll {{设备uuid}}`

- 取消一个设备的授权：

`boltctl forget {{设备uuid}}`

- 显示一个设备的详细信息：

`boltctl info {{设备uuid}}`
