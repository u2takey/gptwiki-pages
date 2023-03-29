# curl 
## chatgpt 
curl 是一个命令行工具，用于通过 HTTP、FTP、SMTP 等协议传输数据。它可以用来从一个 URL 获取文件、发送 HTTP POST 请求、上传文件等操作。

具体来说，curl 命令的常用选项和参数如下：

- `-X` 指定请求的 HTTP 方法（GET、POST、PUT 等）；
- `-d` 指定提交的数据，可以是字符串或者文件；
- `-H` 指定请求头，可以添加多个请求头；
- `-i` 输出 HTTP 响应头；
- `-I` 只输出 HTTP 响应头的第一行（即状态行）；
- `-o` 指定输出文件的名称或路径；
- `-O` 将服务器返回的数据保存到当前目录下的文件，文件名为请求的资源的文件名；
- `-v` 输出详细的调试信息；
- `-s` 静默模式，不输出任何信息；
- `-k` 允许不验证 SSL 证书；
- `-c` 指定 cookie 文件的路径；
- `-b` 指定 cookie 字符串；
- `-A` 指定用户代理；
- `-u` 指定用户名和密码。

使用 curl 命令时，我们需要指定要请求的 URL，以及一些选项和参数，例如：

```bash
$ curl http://example.com
```

这条命令会向 `http://example.com` 发送 GET 请求，并输出服务器返回的响应内容。如果要输出响应头和响应体，可以使用 `-i` 选项：

```bash
$ curl -i http://example.com
```

除了 GET 请求，我们还可以发送 POST 请求，例如：

```bash
$ curl -X POST -d "username=admin&password=123456" http://example.com/login
```

这条命令会向 `http://example.com/login` 发送 POST 请求，提交的数据为 `username=admin&password=123456`。如果服务器需要验证，我们还可以使用 `-u` 选项指定用户名和密码：

```bash
$ curl -u admin:123456 http://example.com/private
```

这条命令会向 `http://example.com/private` 发送 GET 请求，并在请求头中添加 `Authorization` 字段，以验证用户身份。其他的选项和参数可以根据需要进行调整。 

## tldr 
 
> 向 / 从一个服务器传输数据。
> 支持大多数协议，包括 HTTP, FTP, 和 POP3.
> 更多信息：<https://curl.se>.

- 将指定 URL 的内容下载到文件：

`curl {{http://example.com}} --output {{文件名}}`

- 将文件从 URL 保存到由 URL 指示的文件名中：

`curl --remote-name {{http://example.com/filename}}`

- 下载文件，跟随 重定向，并且自动 续传（恢复）前序文件传输：

`curl --remote-name --location --continue-at - {{http://example.com/filename}}`

- 发送表单编码数据（`application/x-www-form-urlencoded` 的 POST 请求）：

`curl --data {{'name=bob'}} {{http://example.com/form}}`

- 发送带有额外请求头，使用自定义请求方法的请求：

`curl --header {{'X-My-Header: 123'}} --request {{PUT}} {{http://example.com}}`

- 发送 JSON 格式的数据，并附加正确的 `Content-Type` 请求头：

`curl --data {{'{"name":"bob"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/users/1234}}`

- 使用用户名和密码，授权访问服务器：

`curl --user myusername:mypassword {{http://example.com}}`

- 为指定资源使用客户端证书和密钥，并且跳过证书验证：

`curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://example.com}}`
