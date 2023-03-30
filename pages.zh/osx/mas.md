# mas 
## chatgpt 
mas是一个用于在macOS上管理Mac App Store的命令行工具。它允许用户通过终端窗口来安装、更新、卸载应用程序，以及查看应用程序的详细信息。

下面是一些常用的mas命令：

- mas search [应用程序名称]: 在Mac App Store中搜索应用程序
- mas list: 列出已安装的应用程序
- mas outdated: 列出需要更新的应用程序
- mas upgrade [应用程序ID]: 更新指定的应用程序
- mas install [应用程序ID]: 安装指定的应用程序
- mas uninstall [应用程序ID]: 卸载指定的应用程序

要使用mas命令，您需要首先安装它。您可以使用Homebrew来安装它。执行以下命令即可：

```
brew install mas
```

安装完成后，您可以使用上述命令来管理Mac App Store上的应用程序。 

## tldr 
 
> Mac 应用商店的命令行界面。
> 更多信息：<https://github.com/mas-cli/mas>.

- 首次登录 Mac 应用商店：

`mas signin {{user@example.com}}`

- 显示所有已安装的应用程序和它们的产品标识符：

`mas list`

- 搜索一个应用程序，在结果旁边显示价格：

`mas search {{应用程序}} --price`

- 安装或更新一个应用程序：

`mas install {{产品标识符}}`

- 安装所有待定的更新：

`mas upgrade`
