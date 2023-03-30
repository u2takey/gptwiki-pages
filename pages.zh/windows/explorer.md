# explorer 
## chatgpt 
explorer命令是Windows系统的一个命令行工具，用于打开资源管理器窗口，浏览和管理文件和文件夹。

使用explorer命令可以在命令行中打开一个新的资源管理器窗口，并定位到指定的文件或者文件夹。该命令还可以用于打开一个指定网址的Internet资源管理器窗口，控制面板或者计算机管理窗口。

explorer命令可以带有各种选项和参数，如：

1. /root – 定义explorer窗口的根文件夹；
2. /select – 定义要在资源管理器窗口中选择的文件或者文件夹；
3. /n – 打开一个新的资源管理器窗口而不是在现有窗口中打开文件或文件夹。

举个例子，如果要在资源管理器中打开名为"D:\example"的文件夹，可以使用以下命令：

explorer D:\example

如果要在资源管理器中选定名为"example.txt"的文件，可以使用以下命令：

explorer /select,C:\example\example.txt

总之，使用explorer命令可以方便地在命令行中管理和查看文件系统，提高工作效率。 

## tldr 
 
> Windows 文件资源管理器。
> 更多信息：<https://ss64.com/nt/explorer.html>.

- 打开 Windows 文件资源管理器：

`explorer`

- 在当前目录打开 Windows 文件资源管理器：

`explorer .`

- 在指定目录打开 Windows 文件资源管理器：

`explorer {{path/to/directory}}`
