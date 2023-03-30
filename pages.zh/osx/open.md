# open 
## chatgpt 
“open”是一个终端命令，可以在 macOS 和 Linux 系统中使用。它用于打开一个文件、文件夹、应用程序等。

命令格式：
```
open [OPTIONS] [file(s)/folder(s)/application(s)]
```

常用选项列表：
- -a：指定应用程序打开文件。例如，“open -a TextEdit myfile.txt” 将使用 TextEdit 应用程序打开 myfile.txt 文件。
- -e：在文本编辑器中打开文件。例如，“open -e myfile.txt” 将使用默认文本编辑器打开 myfile.txt 文件。
- -R：在 Finder 中打开文件或目录并选中它。例如，“open -R myfile.txt” 将在 Finder 中打开 myfile.txt 文件。
- -n：强制打开新的实例，即使已经有一个实例在运行。例如，“open -n TextEdit” 将打开一个新的 TextEdit 实例。
- -F：在“全屏模式”中打开应用程序。例如，“open -F Safari” 将在全屏模式下启动 Safari。
- -b：指定打开应用程序的 bundle identifier，而不是应用程序名称。例如，“open -b com.apple.iTunes” 将打开 iTunes 应用程序。

一些使用 open 命令的例子：
- “open myfile.txt” 将使用默认应用程序打开 myfile.txt 文件。
- “open /Applications/Safari.app” 将打开 Safari 应用程序。
- “open ~/Documents” 将打开 Documents 文件夹。
- “open -a TextEdit ~/Desktop/myfile.txt” 将使用 TextEdit 应用程序打开位于桌面上的 myfile.txt 文件。 

## tldr 
 
> 打开文件、目录和应用程序。
> 更多信息：<https://ss64.com/osx/open.html>.

- 使用系统关联的应用程序打开文件：

`open {{filename.extension}}`

- 运行图形化的 macOS 应用程序：

`open -a {{应用程序名}}`

- 运行指定 包名 的图形化 macOS 应用程序（请参阅`OSascript`命令，查询如何获取应用程序的 包名）：

`open -b {{com.domain.application 应用程序包名}}`

- 在"访达（finder）"中打开当前文件夹：

`open .`

- 打开"访达（finder）", 并且给出指定文件：

`open -R {{文件路径}}`

- 使用系统默认应用程序，打开当前目录中所有给定扩展名的文件：

`open {{*.extension}}`
