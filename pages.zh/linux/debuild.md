# debuild 
## chatgpt 
debuild是Debian Linux操作系统中的一个命令，用于构建软件包。它是Debian构建系统（DBS）的一部分。Debian构建系统是Debian软件包维护工具的组成部分，它能够自动启动多个构建任务，并生成软件包。

debuild命令从源代码或源代码中的Debian包构建Debian软件包。debmake和dh_make等工具可以用来创建Debian包的初始结构。然后，debuild命令可以使用这些文件和其它必需的信息来创建二进制软件包。

debuild命令支持以下选项：

- -S：构建源代码软件包。
- -sa：在构建源代码软件包时，包含原始源码文件。
- -sd：在构建源代码软件包时，不包含原始源码文件。
- -us：跳过对源代码软件包的完整性检查。
- -uc：跳过对源代码软件包的版本控制检查。
- -b：构建二进制软件包。

例如，要构建一个二进制软件包，可以使用以下命令：

debuild -b

此命令将自动下载源代码，并从源代码构建一个二进制软件包。它通常生成一个.deb文件，该文件可以安装到Debian Linux系统中。 

## tldr 
 
> 从源代码构建 `Debian` 软件包的工具。
> 更多信息：<https://manpages.debian.org/debuild>.

- 在当前目录中生成软件包：

`debuild`

- 仅构建二进制包：

`debuild -b`

- 生成软件包后，不运行 `lintian`（检查常见打包错误）：

`debuild --no-lintian`
