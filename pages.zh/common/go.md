# go 
## chatgpt 
go是一种编程语言，也是Go编程语言的编译器和工具。go命令是使用Go编程语言的主要命令之一，它用于构建、测试、安装和管理Go程序和包。下面是一些常用的go命令及其功能：

1. go build - 用于编译Go程序，生成可执行文件或共享库文件。
2. go run - 快速编译和运行Go程序，无需生成可执行文件。
3. go fmt - 格式化Go代码的工具，用于统一代码风格和编码规范。
4. go test - 用于运行Go测试程序，测试Go程序的正确性和性能。
5. go install - 用于安装Go程序或库，将编译好的可执行文件或库安装到系统目录中。
6. go get - 用于下载和安装Go的第三方库或工具，从远程版本控制存储库下载代码并将其安装到系统中。
7. go mod - 当前流行的包管理工具，可以跟踪依赖项、管理版本和构建可复现的Go应用程序或库。
8. go doc - 查询Go函数或语句的文档和用法。

除了以上命令，go还有其他命令和子命令，如go vet用于检查Go程序的静态错误；go runescape用于在Runescape中运行Go程序等。总之，go命令是Go编程语言的重要组成部分，使用它可以简洁、高效地完成Go开发中的各种任务。 

## tldr 
 
> 管理 Go 源代码的工具。
> 此命令也有关于其子命令的文件，例如：`go build`.
> 更多信息：<https://golang.org>.

- 下载并安装由其路径指定的包：

`go get {{路径/到/包}}`

- 编译并运行一个源文件（它必须包含一个 `main` 包）：

`go run {{文件.go}}`

- 将源文件编译为当前命名的可执行文件：

`go build -o {{可执行文件}} {{文件.go}}`

- 编译当前目录中的包：

`go build`

- 执行当前包中的所有测试用例（文件必须以 `_test.go` 结尾）：

`go test`

- 编译并安装当前包：

`go install`

- 在当前目录下初始化一个新模块：

`go mod init {{模块}}`
