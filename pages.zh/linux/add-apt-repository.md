# add-apt-repository 
## chatgpt 
add-apt-repository 是一个 Ubuntu/Debian 系统下的命令，用于向系统的软件仓库添加一个第三方仓库，以便于执行 apt-get 工具安装第三方软件。它的作用是向 /etc/apt/sources.list.d 目录下添加一个新的软件源列表文件。

具体而言，add-apt-repository 会执行以下步骤：

1. 根据参数中的 PPA（Personal Package Archive）地址，在 /etc/apt/sources.list.d 目录下创建一个新的仓库源列表文件，以便运行 apt-get 命令从这个仓库中获取软件包。

2. 如果系统中没有安装相关的公钥，add-apt-repository 也会自动下载并加入到系统的信任列表中，以确保软件包的可信度。

用法示例：

$ sudo add-apt-repository ppa:webupd8team/java

这个命令会添加一个名为 "webupd8team/java" 的 PPA，其中包含 Java 8 的最新版本。然后系统会自动更新仓库信息，可以使用 apt-get 命令直接安装 Java 8：

$ sudo apt-get update
$ sudo apt-get install oracle-java8-installer

需要注意的是，使用 add-apt-repository 添加第三方仓库时需要谨慎，应该只添加可信的、已经过测试的仓库，以免引入安全和稳定性问题。 

## tldr 
 
> apt 仓库管理。
> 更多信息：<https://manned.org/apt-add-repository>.

- 添加一个新的 apt 仓库：

`add-apt-repository {{指定仓库}}`

- 移除一个 apt 仓库：

`add-apt-repository --remove {{指定仓库}}`

- 添加一个仓库并更新缓存：

`add-apt-repository --update {{指定仓库}}`

- 允许从指定仓库下载源码：

`add-apt-repository --enable-source {{指定仓库}}`
