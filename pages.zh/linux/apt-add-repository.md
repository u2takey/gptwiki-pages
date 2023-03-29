# apt-add-repository 
## chatgpt 
apt-add-repository 是一个 Linux 命令，它用于将 PPA（Personal Package Archive）存储库添加到 Ubuntu 系统的 APT （Advanced Package Tool）包管理器中。这样做可以让用户通过 apt-get 命令从 PPA 中安装更新的软件包，这些软件包不在系统默认的仓库中。

更具体地说，apt-add-repository 命令会在 /etc/apt/sources.list 文件中添加一个新的存储库条目，该条目包含 PPA 的地址和公共密钥。然后，使用 apt-get update 命令可以更新系统的本地存储库索引。

这个命令的语法为：

```bash
sudo apt-add-repository ppa:<repository_name>
```

其中，<repository_name> 是 PPA 存储库的名称或地址。

例如，如果要将 numix PPA 存储库添加到 Ubuntu 系统中，可以使用以下命令：

```bash
sudo apt-add-repository ppa:numix/ppa
```

该命令会将以下行添加到 /etc/apt/sources.list 文件中：

```bash
deb http://ppa.launchpad.net/numix/ppa/ubuntu focal main
# deb-src http://ppa.launchpad.net/numix/ppa/ubuntu focal main
```

注意，在添加 PPA 存储库之前，您应该确保它可靠且不会破坏您的系统。并且使用 PPAs 时需要自己承担一定的风险和责任。 

## tldr 
 
> 管理 apt 仓库。
> 更多信息：<https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

- 添加一个 apt 仓库：

`apt-add-repository {{repository_spec}}`

- 移除一个 apt 仓库：

`apt-add-repository --remove {{repository_spec}}`

- 添加一个 apt 仓库之后更新包缓存：

`apt-add-repository --update {{repository_spec}}`

- 开启源码包：

`apt-add-repository --enable-source {{repository_spec}}`
