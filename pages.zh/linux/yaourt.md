# yaourt 
## chatgpt 
yaourt 是一个 Arch Linux 上的一个 AUR (Arch User Repository) 辅助工具，它允许用户方便地从 AUR 中安装和管理软件包。

使用 yaourt 命令可以进行以下操作：

1.搜索 AUR 中的软件包：yaourt <package name>
2.安装软件包：yaourt -S <package name>
3.卸载软件包：yaourt -R <package name>
4.更新已安装的软件包：yaourt -Syu
5.构建和安装 AUR 中的软件包：yaourt -S <AUR package name>
6.清理已安装但不需要的依赖项：yaourt -Sc

需要注意的是，yaourt 已经被官方废弃，并且在 Arch Linux 所有的应用仓库中已被移除，建议使用其他软件来管理 AUR 中的软件包。 

## tldr 
 
> Arch Linux 中用于从 Arch User Repository 中构建软件包的工具。
> 更多信息：<https://linuxcommandlibrary.com/man/yaourt>.

- 同步并更新所有软件包（包括 AUR）：

`yaourt -Syua`

- 安装一个新的软件包（包括 AUR）：

`yaourt -S {{软件包}}`

- 移除一个软件包和它的依赖（包括 AUR 软件包）：

`yaourt -Rs {{软件包}}`

- 在软件包数据库中搜索一个关键字（包括 AUR）：

`yaourt -Ss {{软件包}}`

- 列出已安装的软件包、版本和仓库（AUR 软件包将被列在 'local' 仓库下）：

`yaourt -Q`
