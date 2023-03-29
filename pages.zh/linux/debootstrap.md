# debootstrap 
## chatgpt 
debootstrap是Linux中的一个命令行工具，用于安装Debian或其他基于Debian的发行版的基础文件系统。它可以在不使用安装程序的情况下创建一个新的基础系统。它通常用于创建chroot环境，以便在同一系统上运行多个独立的软件实例。

使用debootstrap的基本语法是：

debootstrap distribution /target [mirror]

其中，distribution是要安装的发行版的名称，/target是要将文件系统安装到的目标目录，mirror是可选的镜像服务器地址。例如，要安装Debian 10（Buster）到目录/my-new-os，可以使用以下命令：

sudo debootstrap buster /my-new-os

使用debootstrap创建的最小系统默认只包含核心安装程序和最基本的软件包。您可以通过安装其他软件包来扩展系统。例如，要安装SSH服务器，请使用以下命令：

sudo chroot /my-new-os
apt-get update
apt-get install openssh-server

这将进入新系统中并使用apt-get命令安装openssh-server软件包。

总之，debootstrap是一个非常有用的命令行工具，可用于创建轻量级、定制化的Linux基础系统，以及在同一系统上运行多个独立的软件实例。 

## tldr 
 
> 创建一个基本的 `Debian` 系统。
> 更多信息：<https://wiki.debian.org/Debootstrap>.

- 在 `debian-root` 目录中创建一个 `Debian` 稳定分支系统：

`sudo debootstrap stable {{path/to/debian-root/}} http://deb.debian.org/debian`

- 使用本地镜像在 `focal-root` 目录中创建一个 `Ubuntu 20.04` 系统：

`sudo debootstrap focal {{path/to/focal-root/}} {{file:///path/to/mirror/}}`

- 切换到可引导系统：

`sudo chroot {{path/to/root}}`

- 列出可用的版本：

`ls /usr/share/debootstrap/scripts/`
