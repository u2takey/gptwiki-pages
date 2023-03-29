# apt-cache 
## chatgpt 
apt-cache 是一个用于管理 Debian/Ubuntu Linux 软件包的命令行工具，可以用来查询软件包信息、依赖关系、搜索软件包等操作。

常用选项和用法：

- apt-cache search <keyword>：搜索关键字相关的软件包。
- apt-cache show <package>：显示安装包的详细信息，包括软件包名、版本、大小、依赖关系、安装位置等。
- apt-cache depends <package>：显示软件包所依赖的其他包。
- apt-cache rdepends <package>：显示依赖于指定软件包的其他包，即反向依赖。
- apt-cache policy <package>：查看软件包的安装策略，包括其来源、版本等信息。
- apt-cache madison <package>：列出软件包在各个仓库中的版本信息并排序，可以用来判断软件包版本是否最新。
- apt-cache pkgnames：列出仓库中所有的软件包名称。

使用 apt-cache 命令需要注意以下几点：

- apt-cache 命令必须和 sudo 或者 root 用户一起使用。
- 它只能查询已经添加到自己的软件仓库列表中的软件包信息。
- 某些操作可能需要联网访问，因为它需要访问软件源来获取信息。 

## tldr 
 
> Debian 和 Ubuntu 的包查询工具。
> 更多信息：<https://manpages.debian.org/latest/apt/apt-cache.8.html>.

- 在当前的软件源中查找一个软件包：

`apt-cache search {{软件包}}`

- 显示指定软件包的相关信息：

`apt-cache show {{软件包}}`

- 查看一个软件包是否安装或是否为最新：

`apt-cache policy {{软件包}}`

- 显示一个软件包的依赖项：

`apt-cache depends {{软件包}}`

- 列出依赖指定软件包的所有软件包：

`apt-cache rdepends {{软件包}}`
