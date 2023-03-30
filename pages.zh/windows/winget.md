# winget 
## chatgpt 
winget 是 Windows Package Manager 的简写，是 Microsoft 推出的一个开源的包管理器，它为 Windows 用户提供了一种快速管理和安装软件包的方式。使用 winget，用户可以搜索、安装、卸载和更新软件包，同时可以方便地管理软件包应用的版本，减少了手动下载、安装和更新软件的时间和成本。

具体来说，winget 可以实现以下功能：

1. 检索软件：用户可以使用 winget 搜索对应的软件包名称、发布者或关键词来查找软件。

2. 安装软件：使用者可以通过 winget install 命令进行单软件的安装，或者使用 winget import 命令导入多个软件包进行批量安装。

3. 卸载软件：使用 winget uninstall 命令可以卸载指定的软件包。

4. 更新软件：使用 winget upgrade 命令可以快速升级已经安装的软件包。

5. 导出或导入软件列表：用户可以使用 winget export 命令将本地的已安装软件包列表导出，并使用 winget import 命令将软件包列表导入到另一台电脑。

总的来说，winget 为 Windows 应用程序管理带来了便捷性和更高的效率。它可以帮助用户自动更新软件、防止应用冲突、提高版本管理、改善软件的可靠性等等。 

## tldr 
 
> Windows 软件包管理器命令行工具。
> 更多信息：<https://learn.microsoft.com/windows/package-manager/winget>.

- 安装一个软件包：

`winget install {{package}}`

- 显示关于一个软件包的信息：

`winget show {{package}}`

- 查找一个软件包：

`winget search {{package}}`
