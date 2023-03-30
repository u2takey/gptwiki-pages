# networksetup 
## chatgpt 
networksetup 是一个在 Mac 上可用的命令行工具，用于管理各种网络设置。它可以用于配置和控制网络接口、IP 地址、DNS、VPN、代理等网络服务和协议。

一些常见的 networksetup 命令选项包括：

- `-listnetworkserviceorder`：列出网络服务的顺序
- `-getinfo`：获取特定网络服务的基本信息，如网络配置、IP 地址、路由器、DNS 等
- `-setdhcp`：设置网络服务使用 DHCP 获取 IP 地址
- `-setmanualwithaddress`：设置网络服务使用手动分配的 IP 地址、子网掩码、路由器地址和 DNS 服务器地址
- `-setdnsservers`：设置网络服务的 DNS 服务器地址
- `-setwebproxy`：设置网络服务的 Web 代理服务器地址和端口
- `-setvpnconfiguration`：设置 VPN 连接配置信息

通过 networksetup 命令，用户可以在终端界面下进行各种网络设置，避免需要打开系统偏好设置界面来操作，提高了效率和便捷性。 

## tldr 
 
> 网络系统首选项配置工具。
> 更多信息：<https://support.apple.com/guide/remote-desktop/about-networksetup-apdd0c5a2d5/mac>.

- 列出可用的网络服务源（以太网、Wi-Fi、蓝牙等）：

`networksetup -listallnetworkservices`

- 显示特定网络设备的配置信息：

`networksetup -getinfo "{{Wi-Fi}}"`

- 获取当前连接的 Wi-Fi 网络名称（Wi-Fi 设备通常为 en0 或 en1）：

`networksetup -getairportnetwork {{en0}}`

- 连接到给定的 Wi-Fi 网络 Connect to a particular Wi-Fi network：

`networksetup -setairportnetwork {{en0}} "{{无线网 SSID}}" {{密码}}`
