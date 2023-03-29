# acme.sh --dns 
## chatgpt 
acme.sh是一个可以为您的网站自动生成SSL证书的自动化脚本。而“--dns”标识是用来指定您想要使用的DNS解析器。

使用这个标识时，您可以将自己的DNS解析器配置到acme.sh中，以便在自动生成SSL证书时，acme.sh可以自动更新您的DNS记录，验证您的域名所有权，然后自动生成SSL证书。

要使用此标识，请在acme.sh命令后输入您想要使用的DNS解析器的名称。例如：

acme.sh --dns dns_aliyun

这将使用阿里云DNS解析器来自动更新您的DNS记录并生成SSL证书。您可以在acme.sh官方网站上找到支持的DNS解析器列表。 

## tldr 
 
> 使用 DNS-01 挑战来签发 TLS 证书。
> 更多信息：<https://github.com/acmesh-official/acme.sh/wiki>.

- 使用自动 DNS API 模式签发证书：

`acme.sh --issue --dns {{gnd_gd}} --domain {{example.com}}`

- 使用自动 DNS API 模式签发通配符证书（用星号表示）：

`acme.sh --issue --dns {{dns_namesilo}} --domain {{example.com}} --domain {{*.example.com}}`

- 使用 DNS 别名模式签发证书：

`acme.sh --issue --dns {{dns_cf}} --domain {{example.com}} --challenge-alias {{alias-for-example-validation.com}}`

- 在添加 DNS 记录后，通过指定自定义的等待时间（秒），在禁用 Cloudflare / Google DNS 自动轮询的同时签发证书：

`acme.sh --issue --dns {{dns_namecheap}} --domain {{example.com}} --dnssleep {{300}}`

- 使用手动 DNS 模式签发证书：

`acme.sh --issue --dns --domain {{example.com}} --yes-I-know-dns-manual-mode-enough-go-ahead-please`
