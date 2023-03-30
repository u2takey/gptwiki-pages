# sw_vers 
## chatgpt 
sw_vers是一个命令行程序，可用于显示当前系统的版本信息。 

当在终端中运行sw_vers时，它将输出以下信息： 

```
ProductName:    macOS
ProductVersion: 11.4
BuildVersion:   20F71
```

其中，`ProductName`是当前操作系统的名称，`ProductVersion`是操作系统的版本号，`BuildVersion`是操作系统的内部版本编译号。 

此命令可用于检查当前系统的版本信息，以确保软件或应用程序的兼容性。 也可用于脚本中自动化检查操作系统版本的过程。 

## tldr 
 
> 打印 macOS 操作系统的版本信息。
> 更多信息：<https://ss64.com/osx/sw_vers.html>.

- 打印所有可用信息（操作系统名称、版本号和构建版本）：

`sw_vers`

- 只打印操作系统的版本号：

`sw_vers -productVersion`

- 只打印构建版本的标识符：

`sw_vers -buildVersion`
