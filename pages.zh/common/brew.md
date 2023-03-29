# brew 
## chatgpt 
brew是一个命令行工具，用于在macOS上安装和管理软件包。它是一个开源项目，由Homebrew社区维护。

可以使用brew命令执行以下操作：

1. 安装软件包：使用brew install命令可以安装基于源代码的软件包。例如，如果要安装Git，可以使用命令brew install git.

2. 升级软件包：使用brew upgrade命令可以升级安装的软件包到最新版本。例如，如果要升级Git，可以使用命令brew upgrade git.

3. 卸载软件包：使用brew uninstall命令可以卸载已安装的软件包。例如，如果要卸载Git，可以使用命令brew uninstall git.

4. 搜索软件包：使用brew search命令可以搜索可用的软件包。例如，如果要搜索关于Python的软件包，可以使用命令brew search python.

5. 显示已安装的软件包：使用brew ls命令可以显示已安装的软件包。例如，如果要显示所有已安装的软件包，可以使用命令brew ls.

总之，brew命令是管理macOS上的软件包的非常方便和强大的工具。 

## tldr 
 
> Linux 和 macOS 的包管理器。
> 更多信息：<https://brew.sh>.

- 安装最新稳定版的配方（formula）或木桶（cask），使用 `--devel` 安装开发版：

`brew install {{配方}}`

- 列出所有已安装的配方和木桶：

`brew list`

- 升级已安装的配方或木桶（如果没有指定，则升级所有已安装的配方/木桶）：

`brew upgrade {{配方}}`

- 从 Homebrew 源存储库中获取最新版本的 Homebrew 以及所有配方和木桶：

`brew update`

- 显示有新版本的配方和木桶：

`brew outdated`

- 搜索可用的配方（即包）和木桶（即原生包）：

`brew search {{包名}}`

- 显示有关配方或木桶的信息（版本、安装路径、依赖等）：

`brew info {{配方}}`

- 检查本地 Homebrew 安装包是否有潜在问题：

`brew doctor`
