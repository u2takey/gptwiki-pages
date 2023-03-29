# go doc 
## chatgpt 
`go doc`是Go语言提供的一个命令行工具，用于查看Go包的文档信息。通过使用该命令，开发者可以很方便地查看Go语言自带和第三方包的API文档和相关说明。

具体而言，执行`go doc <package>`命令将会打印出指定Go包的文档信息。如果不指定`<package>`参数，则会输出Go语言的完整文档信息索引。在文档信息中，包括该包的名称、包的简介、包内的各个函数、变量、常量的详细说明，以及关于该包的使用示例和相关代码示例。

此外，`go doc`还支持通过`-all`选项查看所有Go语言的自带包的文档信息。通过`-http`选项，开发者可以在本地启动一个Web服务，查看Go语言的完整文档信息。例如，`go doc -http=:8080`将会启动一个在本地8080端口上的文档Web服务。开发者可以通过浏览器访问该服务，查看Go语言的完整文档信息。

总之，`go doc`命令是Go语言非常有用的命令行工具之一，帮助开发者快速查看和理解Go语言标准库和第三方包的API文档和相关说明。 

## tldr 
 
> 显示包或符号的文档。
> 更多信息：<https://golang.org/cmd/go/#hdr-Show_documentation_for_package_or_symbol>.

- 显示当前包的文档：

`go doc`

- 显示包文档及导出符号：

`go doc {{encoding/json}}`

- 同时显示符号的文档：

`go doc -all {{encoding/json}}`

- 同时显示源代码：

`go doc -all -src {{encoding/json}}`

- 显示指定的符号：

`go doc -all -src {{encoding/json.Number}}`
