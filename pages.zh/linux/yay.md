# yay 
## chatgpt 
抱歉，yay不是一个Linux系统默认的命令。然而，如果你安装了Arch Linux或者Manjaro Linux发行版，你可以使用yay进行包管理。yay是一个AUR(Arch User Repository)助手，可以帮助你从AUR在线包仓库安装软件包或者更新已安装的包。以下是yay的使用方法：

- 安装yay: 
可以使用pacman命令安装yay：sudo pacman -S yay
- 更新yay:
yay -Syu
- 搜索软件包:
yay -Ss <package_name>
- 安装软件包:
yay -S <package_name>
- 同步AUR：
yay -Sy
- 删除软件包:
yay -R <package_name> 
- 清理AUR缓存:
yay -Yc 

请注意，yay命令的使用情况可能因不同的Linux发行版而异。 

## tldr 
 
> Yet Another Yogurt: 一个用于 Arch Linux 的工具，用于从 Arch User Repository 中构建和安装软件包。
> 另见 `pacman`。
> 更多信息：<https://github.com/Jguer/yay>.

- 从仓库和 AUR 中交互式搜索和安装软件包：

`yay {{软件包|搜索词}}`

- 同步并更新所有来自仓库和 AUR 的软件包：

`yay`

- 只同步和更新 AUR 软件包：

`yay -Sua`

- 从仓库和 AUR 中安装一个新的软件包：

`yay -S {{软件包}}`

- 从仓库和 AUR 中搜索软件包数据库中的关键词：

`yay -Ss {{关键词}}`

- 显示已安装软件包和系统健康状况的统计数据：

`yay -Ps`
