# code 
## chatgpt 
code是一种命令行工具，它是Visual Studio Code编辑器的命令行接口。

当在终端中输入"code"并按下回车时，它会打开Visual Studio Code，并允许你通过命令行接口执行各种操作。

这些操作可以是打开文件、搜索代码、启动调试器、安装插件等。

一些常见的命令行参数：

- -r, --reuse-window：尝试重用已经存在的Visual Studio Code窗口。
- -d, --diff <file>：打开一个文件或Git提交与当前工作空间进行对比。
- -h, --help：显示帮助信息。

除了在终端中使用外，"code"还可以在shell脚本和其他自动化工具中使用。 

## tldr 
 
> Visual Studio Code.
> 更多信息：<https://github.com/microsoft/vscode>.

- 打开 VS Code：

`code`

- 在 VS Code 中打开当前目录：

`code .`

- 在 VS Code 打开一个文件或目录：

`code {{路径/文件或目录}}`

- 在当前打开的 VS Code 窗口中打开一个文件或目录：

`code --reuse-window {{路径/文件或目录}}`

- 在 VS Code 中对比两个文件：

`code -d {{文件1}} {{文件2}}`

- 用超级用户（sudo）权限打开 VS Code：

`sudo code {{路径/文件或目录}} --user-data-dir`
