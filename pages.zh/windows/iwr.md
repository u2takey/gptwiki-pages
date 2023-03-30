# iwr 
## chatgpt 
iwr是PowerShell中的一个命令，其全称为Invoke-WebRequest。它可用于从Web服务器上发送HTTP、HTTPS、FTP、文件或其他协议的请求，并返回请求中包含的信息。下面是该命令的一些常见用法：

1. 从URL下载文件

iwr https://www.example.com/file.zip -OutFile C:\Downloads\file.zip

2. 在请求中添加标头

iwr https://www.example.com -Headers @{ "Authorization" = "Bearer token" }

3. 发送POST请求并包含数据

iwr https://www.example.com -Method POST -Body @{ "username" = "user"; "password" = "pass" }

4. 发送带有代理的请求

iwr https://www.example.com -Proxy "http://proxy.example.com:8080"

通过iwr命令，可以寻找或上传Web内容，而不必离开PowerShell窗口或在浏览器中访问站点。它是一种方便、强大且灵活的工具。 

## tldr 
 
> 这是 `invoke-webrequest` 命令的一个别名。

- 原命令的文档在：

`tldr invoke-webrequest`
