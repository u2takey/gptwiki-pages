# scutil 
## chatgpt 
scutil是macOS下的系统配置工具，它允许用户读取、修改和测试系统配置。以下是scutil的一些常见用法：

1. 显示电脑的主机名称：

    ```
    scutil --get HostName
    ```

2. 显示电脑的本地主机名：

    ```
    scutil --get LocalHostName
    ```

3. 显示电脑的网际协议 (IP) 地址：

    ```
    scutil --get IPAddress
    ```

4. 显示电脑的路由配置：

    ```
    scutil --get State:/Network/Global/IPv4
    ```

5. 显示网络设置：

    ```
    scutil --nwi
    ```

6. 批量配置DNS服务器：

    ```
    sudo scutil --set DNSServers 8.8.8.8 8.8.4.4
    ```
   
    这将把DNS服务器设置为Google的公共DNS服务器。

7. 配置网络接口

    ```
    sudo scutil --set Setup:/Network/Service/$(networksetup -listallnetworkservices | awk '{print $4}')/IPv4
    ```  
   
    这个命令将配置所选择的网络接口。其中$(networksetup -listallnetworkservices | awk '{print $4}')返回本机当前所有网络服务的名称（例如Wi-Fi），这个名称将被用于配置该网络服务。 设置内容是与IPv4相关的。
   
总的来说，scutil是一个功能强大的命令行工具，可用于配置和管理macOS系统上的网络和其他设置。 

## tldr 
 
> 管理系统配置参数。
> 设置配置时必须是 root 权限。
> 更多信息：<https://ss64.com/osx/scutil.html>.

- 显示 DNS 配置：

`scutil --dns`

- 显示代理配置：

`scutil --proxy`

- 获取计算机名称：

`scutil --get ComputerName`

- 设置计算机名称：

`sudo scutil --set ComputerName {{我的计算机名}}`

- 获取主机名（HostName）：

`scutil --get HostName`

- 设置主机名：

`scutil --set HostName {{hostname}}`
