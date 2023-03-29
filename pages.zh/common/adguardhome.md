# AdGuardHome 
## chatgpt 
AdGuardHome是一款免费的开源DNS服务器软件，可用于阻止广告和追踪器，保护个人隐私和网络安全。AdGuardHome可以在Windows、Linux、macOS和Docker上运行，并可通过浏览器进行配置和管理。

该软件有许多功能，包括:

1. 广告屏蔽器: 将广告屏蔽在DNS查询级别，无需安装浏览器扩展程序或应用程序。

2. 网络保护: 阻止恶意网站、phishing和其他网络攻击。

3. 父母控制: 可以阻止成人内容和其他未适合青少年的网站。

4. 隐私保护: 阻塞追踪器和防止数据泄漏。

5. 自定义规则: 可以添加自定义规则来阻止特定域名或IP地址。

AdGuardHome已经有一个默认的过滤列表，但也可以下载其他的过滤列表和规则，以使网络保护和广告屏蔽更加完善。 除此以外，它还支持DoH (DNS-over-HTTPS), DoT (DNS-over-TLS), 和 DNSCrypt 协议加密方式，更加隐私安全。 

## tldr 
 
> 一款全网广告拦截与反跟踪软件。
> 更多信息：<https://github.com/AdguardTeam/AdGuardHome>.

- 运行 AdGuard Home：

`AdGuardHome`

- 使用给定的配置文件运行 AdGuard Home：

`AdGuardHome --config {{给定的/配置文件.yaml}}`

- 设置存储数据的工作目录：

`AdGuardHome --work-dir {{工作目录/路径}}`

- 安装或卸载 AdGuard Home 的服务：

`AdGuardHome --service {{install|uninstall}}`

- 启动 AdGuard Home 的服务：

`AdGuardHome --service start`

- 刷新 AdGuard Home 服务的设置项：

`AdGuardHome --service reload`

- 停止或重启 AdGuard Home 的服务：

`AdGuardHome --service {{stop|restart}}`
