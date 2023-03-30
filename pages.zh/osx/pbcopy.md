# pbcopy 
## chatgpt 
pbcopy是一个在Mac上专门用于将标准输入或文件内容复制到粘贴板剪贴板的命令。它的作用类似于Ctrl+C或Ctrl+Insert键，将选定信息放入粘贴板。

使用pbcopy命令可以将文本、目录路径、HTML代码、shell命令输出等复制到粘贴板中，方便用户随时粘贴到其他应用程序中。

命令示例：

1. 复制文本文件内容到粘贴板

$ cat file.txt | pbcopy 

2. 复制目录路径到粘贴板

$ pwd | pbcopy 

3. 复制HTML代码到粘贴板

$ cat index.html | pbcopy 

4. 复制shell命令输出到粘贴板

$ ls | pbcopy 

一旦使用pbcopy命令将文本内容复制到粘贴板中，就可以将其黏贴到其他应用程序中，例如TextEdit、Word、PowerPoint、邮件等。此外，可以通过pbpaste命令将粘贴板中的内容转储到终端，并使用命令对其进行操作。 

## tldr 
 
> 将标准输出放入剪贴板（命令行里的 cmd + C）。
> 更多信息：<https://ss64.com/osx/pbcopy.html>.

- 将文件的内容放入剪贴板：

`pbcopy < {{文件}}`

- 将命令的执行结果放入剪贴板：

`find . -type t -name "*.png" | pbcopy`
