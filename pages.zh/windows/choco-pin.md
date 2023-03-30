# choco pin 
## chatgpt 
命令：“choco pin”是Chocolatey软件包管理器的命令之一。它指定特定的软件包版本作为常规安装的版本，并将其“固定”在某个特定版本上。这有助于防止软件包版本之间的不兼容问题以及许多其他潜在的问题。

具体来说，使用choco pin命令可以：

1. 指定一个软件包的版本以进行安装，而不是使用默认的最新版本。
2. 安全地更新所有其他软件包，但特定软件包的版本将保持不变。
3. 防止无意中从另一个可能与原先所需版本不兼容的源安装软件包。

例如，如果你需要固定安装Visual Studio Code的1.55.1版本：

choco pin add -n=vscode -v=1.55.1

这将防止将任何其他版本的Visual Studio Code安装到您的计算机上，包括自动更新。如果您需要取消固定版本，请使用以下命令：

choco pin remove -n=vscode

这将删除固定版本的限制并允许默认的最新软件包版本安装在您的计算机上。 

## tldr 
 
> 使用 Chocolatey 将一个包固定到指定的版本。
> 被固定版本的包会在更新时自动忽略。
> 更多信息：<https://chocolatey.org/docs/commands-pin>.

- 显示被固定的包以及他们对应的版本号：

`choco pin list`

- 将一个包固定至当前版本：

`choco pin add --name {{包名}}`

- 将一个包固定直指定的版本：

`choco pin add --name {{包名}} --version {{版本号}}`

- 移除指定包的固定状态：

`choco pin remove --name {{包名}}`
