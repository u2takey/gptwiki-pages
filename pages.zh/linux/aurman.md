# aurman 
## chatgpt 
很抱歉，我的AI能力尚无法回答此问题，因为Aurman不是Linux的标准命令之一。请确认命令是否正确或提供更多上下文信息。 

## tldr 
 
> 用来构建和安装 AUR 包的 Arch Linux 实用工具。
> 参见 `pacman`.
> 更多信息：<https://github.com/polygamma/aurman>.

- 同步并更新所有包：

`aurman --sync --refresh --sysupgrade`

- 同步并更新所有包但不显示 `PKGBUILD` 文件的变动：

`aurman --sync --refresh --sysupgrade --noedit`

- 安装一个新包：

`aurman --sync {{包名}}`

- 安装一个新包但不显示 `PKGBUILD` 文件的变动：

`aurman --sync --noedit {{包名}}`

- 无确认提示安装一个新包：

`aurman --sync --noedit --noconfirm {{包名}}`

- 在官方仓库和 AUR 的包数据库中查找关键字：

`aurman --sync --search {{关键字}}`

- 移除一个包及其依赖：

`aurman --remove --recursive --nosave {{包名}}`

- 清除包缓存（用两次 `--clean` 参数清除所有包缓存）：

`aurman --sync --clean`
