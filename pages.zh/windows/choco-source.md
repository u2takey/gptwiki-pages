# choco source 
## chatgpt 
命令 "choco source" 用于管理Chocolatey软件包管理器的软件包源。

Chocolatey软件包管理器是一个Windows上的命令行工具，它可以自动化安装、更新、卸载和管理Windows上的软件包。

"choco source" 命令的主要功能是：

1. 列出当前已添加的软件包源。
2. 添加新的软件包源。
3. 删除已添加的软件包源。
4. 设置新的默认软件包源。

使用该命令时，可以使用不同的选项来执行不同的功能。以下是几个常见的选项：

- list：列出当前已存在的软件包源。
- add：添加新的软件包源。
- remove：删除已存在的软件包源。
- enable：启用已存在的软件包源。
- disable：禁用已存在的软件包源。
- priority：更改已存在软件包源的优先级。

例如，要添加一个新的软件包源，使用以下命令：

choco source add -n=mySource -s="https://mySource.example.com/chocolatey"

这会将名为“mySource”的新软件包源添加到Chocolatey软件包管理器中，并将其指向“https://mySource.example.com/chocolatey” URL。用户可以在需要时从新的软件包源中安装软件包。 

## tldr 
 
> 使用 Chocolatey 管理包的源。
> 更多信息：<https://chocolatey.org/docs/commands-source>.

- 列出当前可用的源：

`choco source list`

- 添加一个新的包源：

`choco source add --name {{名称}} --source {{url}}`

- 添加包含凭据的新包源：

`choco source add --name {{名称}} --source {{url}} --user {{用户名}} --password {{密码}}`

- 使用客户端证书添加新的包源：

`choco source add --name {{名称}} --source {{url}} --cert {{证书的路径}}`

- 启用一个包源：

`choco source enable --name {{名称}}`

- 禁用一个包源：

`choco source disable --name {{名称}}`

- 移除一个包源：

`choco source remove --name {{名称}}`
