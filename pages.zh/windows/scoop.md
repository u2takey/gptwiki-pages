# scoop 
## chatgpt 
Scoop是一款Windows下的命令行程序安装器，它的设计初衷是为了方便快捷地安装和管理Windows下的开发者工具、实用工具和一些小型程序。使用Scoop，可以通过命令行快速安装、卸载、更新应用程序，而不需要手动下载和安装。

以下是一些常用的命令：

1. scoop install [package]：用于安装指定的应用程序，[package]指应用程序的名称。

2. scoop uninstall [package]：用于卸载已安装的应用程序，[package]指应用程序的名称。

3. scoop update：更新Scoop本身以及已经安装的所有应用程序。

4. scoop search [package]：查找可用的应用程序，[package]指关键词。

5. scoop list：列出已经安装的所有应用程序。

6. scoop status [package]：查看指定应用程序的状态，[package]指应用程序的名称。

7. scoop bucket：管理存储库（bucket），即应用程序的安装源。

总的来说，Scoop是一款帮助Windows用户快速安装和管理应用程序的好工具，不仅可以提高效率，还能避免手动下载和安装所带来的麻烦。 

## tldr 
 
> Windows 的命令行安装程序。
> 更多信息：<https://scoop.sh>.

- 安装一个包：

`scoop install {{包名}}`

- 删除一个包：

`scoop uninstall {{包名}}`

- 更新所有已安装的包：

`scoop update *`

- 列出所有已安装的包：

`scoop list`

- 显示一个包的信息：

`scoop info {{包名}}`

- 搜索一个包：

`scoop search {{包名}}`

- 移除所有包的旧版本并清理下载缓存：

`scoop cleanup -k *`
