# path 
## chatgpt 
path命令是一个Windows命令，可以用于设置和显示系统路径。

它有两个主要的功能：

1. 显示当前系统的环境变量Path的值，即当前操作系统的搜索路径。

2. 设置环境变量Path的值，以添加新的路径。这使用户可以在这些路径中查找可执行文件，而无需输入完整的路径。

当输入“path”命令时，在命令窗口中会显示当前环境变量Path的值。环境变量Path指定了系统在哪些目录中寻找可执行文件以及相关的应用程序。路径以分号分隔，表示搜索的顺序。例如：

C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem

如果要将新路径添加到环境变量Path中，可以将其设置为具有前缀和后缀的新路径值。例如，如果要添加新路径“D:\Program Files”到环境变量Path中，可以使用以下命令：

set PATH=%PATH%;D:\Program Files

其中，%PATH%表示当前的环境变量Path的值，然后添加分号分隔符和新路径。

请注意，更改环境变量Path可能会影响系统或其他应用程序的正常运行。因此，在更改Path前，请务必备份该变量。 

## tldr 
 
> 显示或设置可执行文件的搜索路径。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/path>.

- 显示当前的路径：

`path`

- 将路径设置为一个或多个以分号分隔的目录：

`path {{目录的路径 1[; 目录的路径 2]}}`

- 将新的目录添加到源路径后：

`path {{目录的路径}};%path%`

- 将命令提示符设置为仅搜索当前目录中的可执行文件：

`path ;`
