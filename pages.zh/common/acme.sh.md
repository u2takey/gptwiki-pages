# acme.sh 
## chatgpt 
acme.sh 是一款自动化 ACME 协议客户端工具，可用于管理和颁发 SSL/TLS 证书。

常见的 acme.sh 命令包括：

1. acme.sh --install

安装 acme.sh 并将必要的脚本和文件复制到系统中。需要以 root 用户身份运行。

2. acme.sh --issue

为网站请求 SSL/TLS 证书。用户需要指定包含域名的文本文件，acme.sh 将会自动验证域名并签发证书。

3. acme.sh --renew

续订证书。acme.sh 将检查证书到期时间并自动续订。

4. acme.sh --install-cert

将证书安装到服务器上。默认安装到 Apache、Nginx、Haproxy 等常见的 Web 服务器上。

5. acme.sh --remove

删除证书。

6. acme.sh --list

列出 acme.sh 管理的所有证书和相关信息。

7. acme.sh --help

显示帮助信息。可以在命令后添加更多参数以获得更详细的帮助文档。

使用 acme.sh 可以免费颁发 Let's Encrypt SSL/TLS 证书，支持自动化验证和续订，为网站提供了更安全的加密保护。 

## tldr 
 
> 实现了 ACME 客户端协议的 shell 脚本，是 certbot 的替代品。
> 另见 `acme.sh dns`。
> 更多信息：<https://github.com/acmesh-official/acme.sh>.

- 使用网站根目录模式签发证书：

`acme.sh --issue --domain {{example.com}} --webroot {{/路径/到/网站根目录}}`

- 使用独立模式和 80 端口为多个域名签发证书：

`acme.sh --issue --standalone --domain {{example.com}} --domain {{www.example.com}}`

- 使用独立 TLS 模式和 443 端口签发证书：

`acme.sh --issue --alpn --domain {{example.com}}`

- 使用运行中的 Nginx 的配置来签发证书：

`acme.sh --issue --nginx --domain {{example.com}}`

- 使用运行中的 Apache 的配置来签发证书：

`acme.sh --issue --apache --domain {{example.com}}`

- 使用自动 DNS API 模式签发一个通配符（\*）证书：

`acme.sh --issue --dns {{dns_cf}} --domain {{*.example.com}}`

- 将证书文件安装到指定位置（对自动更新证书很有用）：

`acme.sh --install-cert -d {{example.com}} --key-file {{/路径/到/example.com.key}} --fullchain-file {{/路径/到/example.com.cer}} --reloadcmd {{"systemctl force-reload nginx"}}`
