# assoc 
## chatgpt 
在Windows操作系统中， assoc命令用于显示或更改文件扩展名和程序之间的关联。

具体来说，该命令用于列出或更改文件扩展名，以及与该扩展名相关联的程序名称。当用户双击该文件时，Windows将自动启动与该扩展名相关联的程序。

例如，如果用户想要打开以“.txt”结尾的文件，并双击该文件，Windows会自动启动关联的文本编辑器程序。assoc命令可用于查看此关联，并更改该关联，以便使用其他程序打开该类型的文件。

要使用assoc命令，请在命令提示符处键入“assoc”命令，后跟文件扩展名，以列出该扩展名相关联的程序。例如：

assoc .txt

将列出“.txt”扩展名相关联的程序。

要更改文件扩展名的关联，请键入“assoc”命令，后跟文件扩展名和新的关联程序名称。例如：

assoc .txt=notepad.exe

将以“Notepad”文本编辑器为新的关联程序来打开以“.txt”为扩展名的文件。 

## tldr 
 
> 显示或修改文件扩展名关联。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/assoc>.

- 显示所有当前文件扩展名关联的列表：

`assoc`

- 显示指定扩展名的关联文件类型：

`assoc {{.txt}}`

- 将文件扩展名与特定的文件类型关联：

`assoc {{.txt}}={{txtfile}}`
