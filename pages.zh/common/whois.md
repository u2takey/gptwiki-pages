# whois 
## chatgpt 
whois是一个Internet协议工具，可用于查询关于特定的IP地址、域名或者ASN号码的注册信息。

该命令的基本语法是: 

whois [options] [search_term]

其中，[options]用于指定需要的选项，而[search_term]则用于指定需要查询的IP地址、域名或ASN号码。

使用whois命令可以获得以下信息：

1.域名的注册商、注册日期、到期日期、DNS服务器列表等等。

2.域名的防止盗用信息，例如域名所有者姓名、地址、电子邮件地址和联系电话。

3. ASN号码的所有者信息，例如自治系统名、自治系统号码、ASN所在地址、ASN注册信息以及相关联系人的信息。

总之，whois命令可用于获取网络域名、服务器和IP地址等相关信息，是维护互联网运行的必要工具之一。 

## tldr 
 
> WHOIS（RFC 3912）协议的命令行客户端。
> 更多信息：<https://github.com/rfc1036/whois>.

- 获取域名信息：

`whois {{example.com}}`

- 获取 IP 地址信息：

`whois {{8.8.8.8}}`

- 获取 IP 地址用于报告滥用的联系方式：

`whois -b {{8.8.8.8}}`
