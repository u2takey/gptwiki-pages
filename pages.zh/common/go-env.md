# go env 
## chatgpt 
命令"go env"用于打印Go环境变量的值。它将显示当前设置的所有环境变量及其值。以下是一些通常显示的环境变量：

- GOARCH：目标机器的体系结构（amd64、arm、386等）
- GOOS：目标操作系统（linux、windows、darwin等）
- GOPATH：工作空间路径
- GOROOT：Go安装目录路径
- GOBIN：Go二进制文件路径

此外，还有许多其他环境变量可用，包括用于编译、运行和测试Go程序的变量。您可以使用"go help env"命令来了解更多关于这些变量的信息。 

## tldr 
 
> 管理 Go 工具链使用的环境变量。
> 更多信息：<https://golang.org/cmd/go/#hdr-Print_Go_environment_information>.

- 显示所有环境变量：

`go env`

- 显示指定的环境变量：

`go env {{GOPATH}}`

- 设置某个环境变量为指定值：

`go env -w {{GOBIN}}={{路径/到/目录}}`

- 重置某个环境变量的值：

`go env -u {{GOBIN}}`
