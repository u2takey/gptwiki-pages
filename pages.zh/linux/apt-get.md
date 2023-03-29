# apt-get 
## chatgpt 
apt-get 是一个命令行工具，用于安装、更新和删除 Linux 操作系统上的软件包（packages）。它的全称是 Advanced Package Tool，它是 Debian 和 Ubuntu 等 Debian 基础的 Linux 发行版中一个非常重要的软件包管理器。

apt-get 命令有许多不同的选项和子命令。下面是一些最常用的：

1. install：安装软件包。

2. remove：删除软件包。

3. update：更新软件包列表。

4. upgrade：升级所有已安装的软件包。

5. dist-upgrade：升级所有已安装的软件包，并处理依赖关系。

6. autoremove：删除废弃的软件包。

7. purge：彻底删除软件包及其配置文件。

8. clean：清除软件包缓存。

例如，要安装 Firefox 浏览器，您可以使用以下命令：

sudo apt-get install firefox

apt-get 命令的优点是其自动处理依赖关系。如果您尝试安装一个软件包，但它依赖于其他软件包，apt-get 会自动安装所有必需的软件包。这样可以省去用户自行下载和安装软件包的麻烦。

总之，apt-get 是一个强大的软件包管理器，可以方便地管理操作系统上的软件包。 

## tldr 
 
> Debian 和 Ubuntu 的软件包管理工具。
> 使用 `apt-cache` 查找包。
> 更多信息：<https://manpages.debian.org/latest/apt/apt-get.8.html>.

- 更新可用软件包及其版本列表（推荐在其他 `apt-get` 命令运行之前使用）：

`apt-get update`

- 安装一个软件包或更新到最新版本：

`apt-get install {{软件包}}`

- 移除一个软件包：

`apt-get remove {{软件包}}`

- 移除一个软件包及其配置文件：

`apt-get purge {{软件包}}`

- 升级所有已安装软件包到最新版本：

`apt-get upgrade`

- 清理本地仓库 - 移除下载中断后无法再继续下载的（`.deb`）包文件：

`apt-get autoclean`

- 移除所有不再需要的软件包：

`apt-get autoremove`

- 升级已安装的软件包（类似于 `upgrade`），移除过时的软件包并安装额外的软件包以满足新的依赖：

`apt-get dist-upgrade`
