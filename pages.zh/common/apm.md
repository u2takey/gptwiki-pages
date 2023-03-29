# apm 
## chatgpt 
apm 是 Atom Package Manager 的缩写，是 Atom 的命令行界面。Atom 是一款免费且开源的文本编辑器，apm 命令可以用于管理 Atom 上安装的插件（即“包”或“包裹”），包括搜索、安装、升级、删除、查看信息等操作。

以下是一些常用的 apm 命令：

- apm search [name]：搜索 Atom 上的插件，可以使用 name 参数来指定插件名称进行搜索
- apm install [name]：安装 Atom 插件，可以使用 name 参数指定插件名称
- apm upgrade [name]：升级指定的 Atom 插件，如果不指定 name 参数，则会升级所有已安装的插件
- apm remove [name]：删除指定的 Atom 插件
- apm list：列出所有已安装的 Atom 插件
- apm view [name]：查看指定 Atom 插件的详细信息

总之，apm 命令可以帮助 Atom 用户轻松管理其使用的插件，使其对编辑器的个性化需求变得更简单易行。 

## tldr 
 
> Atom 编辑器的包管理工具。
> 参见 `atom`.
> 更多信息：<https://github.com/atom/apm>.

- 下载包：http://atom.io/packages 和主题 http://atom.io/themes：

`apm install {{包名}}`

- 移除包 / 主题：

`apm remove {{包名}}`

- 升级包 / 主题：

`apm upgrade {{包名}}`
