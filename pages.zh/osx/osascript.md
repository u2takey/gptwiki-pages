# osascript 
## chatgpt 
osascript是在Mac OS X中使用的命令行工具，用于执行AppleScript脚本以在终端窗口中访问和控制应用程序和系统。以下是osascript的详细解释：

1.	osascript是一个命令行操作系统的工具，它可以在Mac OS X终端窗口中执行一个AppleScript脚本。

2.	osascript可以与其他命令行工具和脚本一起使用，例如shell脚本、Python脚本等。

3.	osascript可以访问和控制Mac OS X系统中的应用程序，例如Finder、iTunes、Safari以及其他一些应用程序。

4.	osascript还可以使用命令行参数来传递脚本中的变量、函数等，并且可以将脚本的输出重定向到文件中。

5.	使用osascript可以自动化某些任务，例如打开应用程序、操作系统窗口、查找文件等，从而提高工作效率。

总之，osascript是一种强大的Mac OS X命令行工具，可以帮助您完成许多自动化任务。 

## tldr 
 
> 在命令行中运行指定的 AppleScript 或 JavaScript 脚本程序。
> 更多信息：<https://ss64.com/osx/osascript.html>.

- 运行一个 AppleScript 命令：

`osascript -e '{{say "你好世界"}}'`

- 运行多条 AppleScript 命令：

`osascript -e '{{say "你好"}}' -e '{{say "世界"}}'`

- 运行一个已编译的脚本（`*.scpt`），包脚本（`*.scptd`），或明文的（`*.applescript`）AppleScript 文件：

`osascript {{目录 / 脚本文件.scpt}}`

- 获取应用程序的包名（这个包名，可以用在命令 `open -b` 中）：

`osascript -e 'id of app "{{应用程序名}}"'`

- 运行一个 JavaScript 命令：

`osascript -l JavaScript -e '{{console.log("你好世界！");}}'`

- 运行 JavaScript 文件：

`osascript -l JavaScript {{路径 / 文件名.js}}`
