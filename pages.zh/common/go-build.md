# go build 
## chatgpt 
go build是Golang编译命令。它用于将Go语言源代码编译成可执行文件或库文件。

当执行`go build`命令时，Go编译器会检查当前目录下的所有Go文件，并把它们编译成一个可执行文件。如果有依赖的第三方库，则也会被编译进可执行文件中。需要注意的是，go build只会编译当前目录下的文件，不会进行递归编译。

默认生成的可执行文件与当前目录中的目录名称相同。例如，当前目录为main，则生成可执行文件名为main。如果需要使用不同的文件名，可以使用`-o`选项来指定。

go build还可以用于编译库文件，通常使用`go build -o libname.a -buildmode=c-archive`来生成静态库。当然，还有其他一些编译选项，如`-ldflags`用于指定编译链接选项，`-a`用于重新编译整个程序等等。

需要注意的是，go build命令仅仅是编译程序，不会进行程序的安装。如果要将编译后的程序安装到系统中，需要使用go install命令。 

## tldr 
 
> 编译 Go 源代码。
> 更多信息：<https://golang.org/cmd/go/#hdr-Compile_packages_and_dependencies>.

- 编译‘package main’文件（输出为不带扩展名的文件名）：

`go build {{路径/到/main.go}}`

- 编译，并指定输出文件名：

`go build -o {{路径/到/二进制文件}} {{路径/到/源文件.go}}`

- 编译一个包：

`go build -o {{路径/到/二进制文件}} {{路径/到/包}}`

- 编译 main 包为可执行文件，并开启数据竞态检测：

`go build -race -o {{路径/到/可执行文件}} {{路径/到/main/包}}`
