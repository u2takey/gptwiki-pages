# aptitude 
## chatgpt 
aptitude是一个在Linux操作系统上的包管理工具，它可以让用户方便地搜索、安装、更新和删除软件包。

通过aptitude可以：

1. 浏览和搜索软件包：用户可以使用aptitude来查看所有可用的软件包，或者搜索特定的软件包。

2. 安装软件包和构建依赖：当用户选择安装软件包时，aptitude将自动下载和安装软件包所需的所有依赖项。

3. 更新软件包：用户可以使用aptitude将系统中已安装的软件包更新到最新版本。

4. 删除软件包：用户可以使用aptitude来删除软件包及其依赖项。

5. 安装软件包的不同版本：用户可以使用aptitude来安装软件包的不同版本，以便测试或回退操作。

6. 显示软件包详细信息：用户可以使用aptitude来查看软件包的详细信息，包括版本号、依赖项、文件列表等。

7. 通过命令行和图形用户界面使用：用户可以在命令行和图形用户界面中使用aptitude。

总之，aptitude是一个强大的命令行工具，能够大大简化Linux用户的包管理任务。 

## tldr 
 
> Debian 和 Ubuntu 上的软件包管理工具。
> 更多信息：<https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

- 同步可用软件包及其版本列表，在运行后续 aptitude 命令前，应该首先运行该命令：

`aptitude update`

- 安装一个新的软件包及其依赖：

`aptitude install {{软件包}}`

- 查找一个软件包：

`aptitude search {{软件包}}`

- 查找一个已安装的软件包（`?installed` 是一个 aptitude 搜索项）：

`aptitude search '?installed({{软件包}})'`

- 移除一个软件包并移除所有依赖它的软件包：

`aptitude remove {{软件包}}`

- 更新已安装软件包到最新版本：

`aptitude upgrade`

- 更新已安装的软件包（类似于 `aptitude upgrade` 命令），移除过时的软件包并安装额外的软件包以满足新的软件包依赖项：

`aptitude full-upgrade`

- 锁定一个已安装的软件包以便阻止它自动升级：

`aptitude hold '?installed({{软件包}})'`
