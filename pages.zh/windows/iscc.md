# iscc 
## chatgpt 
iscc命令是Inno Setup Compiler命令行工具的缩写，用于将Inno Setup脚本编译成可执行安装程序。Inno Setup是一款免费的、可扩展的、易于使用的安装程序制作工具，支持多种操作系统和语言。

iscc命令的基本语法为：

```
iscc [/O [/F[file]]] script_file
```

其中，iscc表示执行iscc命令；/O表示启用优化；/F[file]表示输出文件名，file为可选参数，用于指定输出文件名，如果未指定则使用脚本文件名；script_file表示要编译的Inno Setup脚本文件名。

例如，以下命令将编译名为sample.iss的脚本文件，并输出生成的安装程序文件到当前目录下：

```
iscc sample.iss
```

iscc命令支持多种参数和选项，可用于控制编译过程、指定输出文件名、设置编译器选项、指定编译器版本等。具体的参数和选项可以通过iscc /?命令查看帮助文档。 

## tldr 
 
> Inno Setup 安装程序的编译器。
> 它将 Inno Setup 脚本编译为 Windows 安装程序可执行文件。
> 更多信息：<https://jrsoftware.org/isinfo.php>.

- 编译一个 Inno Setup 脚本：

`iscc {{脚本路径.iss}}`

- 静默编译一个 Inno Setup 安装程序：

`iscc /Q {{脚本路径.iss}}`

- 编译已签名的 Inno Setup 安装程序：

`iscc /S={{名称}}={{命令}} {{脚本路径.iss}}`
