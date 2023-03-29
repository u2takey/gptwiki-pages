# bluetoothctl 
## chatgpt 
bluetoothctl是Linux系统下的一个蓝牙控制工具。它允许用户与蓝牙设备进行交互，可以扫描、连接、配对、管理蓝牙设备等。

具体来说，bluetoothctl命令可以完成以下功能：

1. 打开或关闭蓝牙

使用“power on”命令可以打开蓝牙，使用“power off”命令可以关闭蓝牙。

2. 搜索蓝牙设备

使用“scan on”命令可以搜索周围的蓝牙设备。搜索到的设备及其属性将显示在控制台上。

3. 连接蓝牙设备

使用“connect”命令可以连接到一个蓝牙设备。在连接之前，可以使用“trust”命令来将设备添加到信任列表中。

4. 配对蓝牙设备

使用“pair”命令可以配对一个蓝牙设备。在配对之前，需要先与设备建立连接。

5. 断开蓝牙设备

使用“disconnect”命令可以断开一个已连接的蓝牙设备。

6. 显示已配对的设备列表

使用“paired-devices”命令可以显示已配对的设备列表。

7. 显示当前连接的设备列表

使用“devices”命令可以显示当前连接的设备列表。

8. 显示已连接设备的属性信息

使用“info”命令可以显示已连接设备的属性信息，包括设备名称、MAC地址、信号强度等。

除此之外，bluetoothctl还支持其它一些命令和参数，可以通过“help”命令查看帮助文档。 

## tldr 
 
> 从命令行管理蓝牙设备。
> 更多信息：<https://bitbucket.org/serkanp/bluetoothctl>.

- 进入 bluetoothctl 外壳程序：

`bluetoothctl`

- 列出设备：

`bluetoothctl -- devices`

- 与一个设备配对：

`bluetoothctl -- pair {{mac 地址}}`

- 移除一个设备：

`bluetoothctl -- remove {{mac 地址}}`

- 连接一个已配对的设备：

`bluetoothctl -- connect {{mac 地址}}`

- 断开一个已配对的设备：

`bluetoothctl -- disconnect {{mac 地址}}`
