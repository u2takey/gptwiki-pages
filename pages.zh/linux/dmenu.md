# dmenu 
## chatgpt 
dmenu 是 Linux 系统中的一个动态菜单工具，它可以通过键盘输入和即时搜索来快速选择菜单选项。dmenu 被设计成一个基于文本输入的应用程序选择器，可以使用它来快速启动应用程序、切换窗口、选择电影等。dmenu 可以被用于 Linux 命令行界面，也可以用于窗口管理器中。

dmenu 的基本用法如下：

```
dmenu [options] < prompt_text
```

其中 options 表示 dmenu 的选项，prompt_text 表示在 dmenu 中显示的提示文本。

常用选项：

- -i：忽略大小写进行匹配。
- -l lines：指定 dmenu 中显示的行数。
- -fn font：指定 dmenu 字体。
- -nb color：指定 dmenu 背景色。
- -nf color：指定 dmenu 前景色。
- -sb color：指定选择菜单时的背景色。
- -sf color：指定选择菜单时的前景色。

示例：

1. 启动应用程序

```
dmenu_run
```

2. 在终端中使用 dmenu 运行命令

```
echo -e "one\ntwo\nthree\nfour" | dmenu
```

在输入框中输入相应的字符（例如 o），dmenu 会显示所有包含该字符的选项，然后按下 Enter 键即可执行相应的命令。

3. 在窗口管理器中使用 dmenu

在 i3wm 窗口管理器中，可以使用 dmenu 打开应用程序或执行命令。

```
bindsym $mod+d exec "dmenu_run"
``` 

## tldr 
 
> 动态菜单。
> 根据文本输入创建菜单，其中每一项都在新行中。
> 更多信息：<https://manned.org/dmenu>.

- 显示 `ls` 命令输出的菜单：

`{{ls}} | dmenu`

- 显示包含自定义项目的菜单，并用新行（`\n`）分隔：

`echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu`

- 让用户在多个项目之间进行选择，然后将所选项目保存到文件中：

`echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu > {{color.txt}}`

- 在特定的监视器上启动 `dmenu`：

`ls | dmenu -m {{1}}`

- 在屏幕底部显示 `dmenu`：

`ls | dmenu -b`
