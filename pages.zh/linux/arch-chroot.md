# arch-chroot 
## chatgpt 
arch-chroot 是一个用于切换到另一个 Linux 系统根目录的命令。具体来说，arch-chroot 是 Arch Linux 发行版中提供的一个脚本，可以在系统引导后使用。

使用 arch-chroot 命令可以将用户的工作环境与根目录分离开来，类似于在目标系统上进行操作一样。这对于修复损坏的系统、在另一个文件系统中安装新软件、备份数据等方面非常有用。

使用 arch-chroot 命令时，用户必须指定目标文件系统的根目录。例如，如果用户要使用 /dev/sda6 分区的 Arch Linux 系统，则可以使用以下命令将其挂载到 /mnt 目录：

# mount /dev/sda6 /mnt

接下来，使用以下命令切换到新系统：

# arch-chroot /mnt

这将打开一个新的 Bash 终端窗口，并为用户提供在 Arch Linux 系统下运行命令的权限。在这个新的环境中，用户可以轻松地执行常规操作，例如安装新软件包、修改配置文件或备份重要文件。

完成操作后，用户可以使用 exit 命令退出 arch-chroot 环境。在退出之前，应该确保正确解除挂载目标文件系统：

# umount /mnt

总之，arch-chroot 命令是一个可以帮助用户切换到另一个 Linux 文件系统的实用工具。在操作系统的修复、安装和管理过程中，使用它可以提高工作效率，同时也有助于确保数据的安全性。 

## tldr 
 
> 辅助 Arch Linux 安装流程的更强 `chroot` 命令。
> 更多信息：<https://man.archlinux.org/man/arch-chroot.8>.

- 在新的根目录下开启一个交互外壳程序（默认是 `bash`）：

`arch-chroot {{新根目录}}`

- 指定除当前用户外的其他用户来运行外壳程序：

`arch-chroot -u {{用户名}} {{新根目录}}`

- 在新的根目录下运行一个自定义命令（取代默认的 `bash`）：

`arch-chroot {{新根目录}} {{命令}} {{命令参数}}`

- 指定除默认的 `bash` 以外的外壳程序（以下例子需要现在目标系统中先安装 `zsh`）：

`arch-chroot {{新根目录}} {{zsh}}`
