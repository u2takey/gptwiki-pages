# brew cask 
## chatgpt 
brew cask是Homebrew的一个子命令，可以用于管理和安装Mac的安装包。brew cask是Homebrew的扩展程序，专门用于管理常用的Mac应用程序。

该命令有以下常用的子命令：

1. list：列出已安装的应用程序。
2. search：搜索所有可用的应用程序。
3. install：安装应用程序。
4. uninstall：卸载应用程序。
5. upgrade：升级所有已安装的应用程序。
6. info：获取应用程序的描述信息。

使用brew cask安装应用程序非常容易，例如要安装Google Chrome，只需运行以下命令：

```
brew cask install google-chrome
```

这个命令将从Homebrew Cask存储库中下载Google Chrome安装程序，并安装它。

与其他Homebrew命令一样，使用brew cask命令需要先安装Homebrew。安装Homebrew的方法可以在官方网站上找到：https://brew.sh/。 

## tldr 
 
> macOS 上的应用程序包管理工具。
> 更多信息：<https://github.com/Homebrew/homebrew-cask>.

- 模糊搜索可用命令行工具和软件包：

`brew search {{软件名}}`

- 安装一个软件：

`brew cask install {{软件名}}`

- 列出全部已安装软件：

`brew cask list`

- 列出全部已安装的软件中，可以升级的：

`brew cask outdated`

- 将一个已安装的软件升级到最新的版本：

`brew cask upgrade {{软件名}}`

- 删除一个软件（仅通过 brew cask install 方式安装的）：

`brew cask uninstall {{软件名}}`

- 卸载一个软件并删除相关的设置和文件：

`brew cask zap {{软件名}}`

- 显示指定软件的相关信息：

`brew cask info {{软件名}}`
