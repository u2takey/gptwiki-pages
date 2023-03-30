# systemsetup 
## chatgpt 
systemsetup是一个Mac电脑的命令行工具，它可以访问和更改系统设置和配置信息。以下是systemsetup的常用选项和功能：

- -listallnetworkservices：列出所有的网络服务，例如Wi-Fi、以太网和蓝牙
- -getcomputername：获取Mac电脑的计算机名称
- -setcomputername：更改Mac电脑的计算机名称
- -gethostname：获取Mac电脑的主机名
- -sethostname：更改Mac电脑的主机名
- -getlocalhostname：获取本地主机名
- -setlocalhostname：更改本地主机名
- -gettimezone：获取当前时区
- -settimezone：更改时区
- -getusingnetworktime：查看是否启用了网络时间
- -setusingnetworktime：启用或禁用网络时间
- -getnetworktimeserver：获取网络时间服务器地址
- -setnetworktimeserver：设置网络时间服务器地址
- -getremotelogin：查看是否启用远程登录
- -setremotelogin：启用或禁用远程登录

这些选项和功能可以帮助用户更轻松地管理和配置Mac电脑的系统设置。 

## tldr 
 
> 配置系统首选项计算机设置。
> 更多信息：<https://support.apple.com/guide/remote-desktop/about-systemsetup-apd95406b8d/mac>.

- 启用远程登录（SSH）：

`systemsetup -setremotelogin on`

- 指定时区、NTP 服务器并启用网络时间：

`systemsetup -settimezone {{美国 / 太平洋}} -setnetworktimeserver {{us.pool.ntp.org}} -setusingnetworktime on`

- 使机器从不休眠，并在电源故障或内核死机时自动重新启动：

`systemsetup -setsleep off -setrestartpowerfailure on -setrestartfreeze on`

- disks 选择启动：

`systemsetup -liststartupdisks`

- 指定新的启动盘：

`systemsetup -setstartupdisk {{路径}}`
