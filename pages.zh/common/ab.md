# ab 
## chatgpt 
ab是ApacheBench（Apache测试工具）的缩写，是一个基于命令行的实用工具，用于测试 web 服务器的性能和效率。

该命令的语法如下：

```
ab [options] [http[s]://]hostname[:port]/path
```

其中，[options]是可选参数，[http[s]://]hostname[:port]/path是需要测试的目标 URL，可以包含协议、主机名、端口和路径信息。

ab命令的主要选项包括：

- -n：指定请求总次数；
- -c：指定并发请求数；
- -t：指定测试所进行的最大秒数；
- -p：指定包含 POST 数据的文件路径；
- -T：指定 POST 数据的 Content-type；
- -k：启用 HTTP KeepAlive；
- -S：启用 SSL 安全连接。

除了这些常用选项，还有许多其他选项可以通过 `ab -h` 命令查看。

使用ab命令可以帮助开发人员测试 web 服务器的性能，找出潜在的性能瓶颈，并优化代码以提高网站响应速度和稳定性。 

## tldr 
 
> Apache 基准测试工具。
> 更多信息：<https://httpd.apache.org/docs/current/programs/ab.html>.

- 向目标 URL 执行 100 次 HTTP GET 请求：

`ab -n {{100}} {{url}}`

- 使用 10 个并发请求，同时向目标 URL 执行 100 次 HTTP GET 请求：

`ab -n {{100}} -c {{10}} {{url}}`

- 使用来自文件的 JSON 负载对 URL 执行 100 个 HTTP POST 请求：

`ab -n {{100}} -T {{application/json}} -p {{path/to/file.json}} {{url}}`

- 使用 HTTP [K]eep Alive，即在一个 HTTP 会话中执行多个请求：

`ab -k {{url}}`

- 为基准测试设置最大的测试时间（单位：秒）：

`ab -t {{60}} {{url}}`
