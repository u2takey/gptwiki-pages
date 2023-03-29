# gunicorn 
## chatgpt 
gunicorn是一个Python Web服务器网关接口（WSGI）HTTP服务器，可以将Web应用程序部署到生产环境中。它的主要优点是快速，可扩展性和高负载容量，可以支持多种异步Python Web框架，例如Flask，Django和Bottle等，同时允许使用多个工作进程，提高处理请求的效率。

以下是gunicorn命令的一些常见用法：

1. 启动gunicorn服务器，默认监听8000端口，使用4个工作进程：
```
$ gunicorn myapp:app
```

2. 指定监听的端口和工作进程数量：
```
$ gunicorn -w 4 -b 0.0.0.0:8080 myapp:app
```
在这个示例中，服务器将监听8080端口，并使用4个工作进程。

3. 使用UNIX套接字：
```
$ gunicorn -w 4 -b unix:/tmp/myapp.sock myapp:app
```
在这个示例中，服务器将使用UNIX套接字“/tmp/myapp.sock”进行通信。

4. 定义日志级别和日志文件：
```
$ gunicorn -w 4 -b 0.0.0.0:8080 -t 120 --log-level=info --log-file=/var/log/gunicorn.log myapp:app
```
在这个示例中，服务器将使用级别为info的日志级别，并将日志写入到“/var/log/gunicorn.log”文件中。

5. 使用SSL/TLS加密：
```
$ gunicorn -w 4 -b 0.0.0.0:443 --keyfile=/etc/ssl/private/key.pem --certfile=/etc/ssl/certs/cert.pem myapp:app
```
在这个示例中，服务器将在443端口上监听，并使用“/etc/ssl/private/key.pem”和“/etc/ssl/certs/cert.pem”中的SSL/TLS密钥和证书进行加密通信。

总之，gunicorn是一个易于使用的Web服务器，可以满足日常开发和生产环境中的需要，可以大大提高Web应用程序的性能和可扩展性。 

## tldr 
 
> Python 的 WSGI http 服务器。
> 更多信息：<https://gunicorn.org/>.

- 运行 python web 应用程序：

`gunicorn {{导入路径：应用程序}}`

- 在 localhost 上监听 8080 端口：

`gunicorn --bind {{localhost}}:{{8080}} {{导入路径：应用程序}}`

- 启用实时自动加载：

`gunicorn --reload {{导入路径：应用程序}}`

- 使用 4 个工作进程处理请求：

`gunicorn --workers {{4}} {{导入路径：应用程序}}`

- 使用 4 个工作线程处理请求：

`gunicorn --threads {{4}} {{导入路径：应用程序}}`

- 通过 https 运行应用程序：

`gunicorn --certfile {{cert.pem}} --keyfile {{key.pem}} {{导入路径：应用程序}}`
