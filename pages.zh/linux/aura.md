# aura 
## chatgpt 
很抱歉，作为一位 AI，我不能提供 aura 命令的详细解释，因为在标准 Linux 系统中并没有这个命令，而这可能是您提到的特定工具、软件或脚本。 我建议您检查拼写，或者提供更多上下文和信息，以便我可以更好地帮助您解决问题。 

## tldr 
 
> Aura 包管理器：一个安全且支持多语言的 Arch Linux 和 AUR 的包管理器。
> 更多信息：<https://github.com/fosskers/aura>.

- 从官方仓库和 AUR 检索包：

`aura --aursync --both --search {{包名|正则}}`

- 从 AUR 安装一个软件包：

`aura --aursync {{包名}}`

- 以详细模式升级所有的 AUR 包并移除所有的编译依赖：

`aura --aursync --diff --sysupgrade --delmakedeps --unsuppress`

- 从官方仓库安装一个软件包：

`aura --sync {{包名}}`

- 同步并更新官方仓库的所有软件包：

`aura --sync --refresh --sysupgrade`

- 使用包缓存降级一个软件包：

`aura --downgrade {{包名}}`

- 移除一个软件包及其依赖：

`aura --remove --recursive --unneeded {{包名}}`

- 移除孤儿包（作为依赖安装但现在不被任何包依赖）：

`aura --orphans --abandon`
