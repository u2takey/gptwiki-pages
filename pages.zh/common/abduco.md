# abduco 
## chatgpt 
abduco 是一个类似于 GNU Screen 或 Tmux 的终端复用程序，它可以让用户在不同的窗口或会话之间切换，使用 abduco 可以避免打开多个终端来执行不同的任务。

下面是 abduco 命令的详细解释：

用法：abduco [-A] [-c 名称] [-e 程序] [-n 名称] [-r 标志] [-t 标签] [ -v ]  命令

选项和参数：

-A：将选项传递给下一个要绑定到的会话。
-c：恢复指定名称的会话。
-e：在新会话上运行指定程序。
-n：使用指定名称创建新的会话。
-r：为会话设置指定标志。
-t：指定标签名称。
-v：显示版本信息。

示例：

1. 创建一个新会话：

$ abduco -c mysession

2. 创建一个新会话，使用指定的程序：

$ abduco -n mysession -e vim

3. 恢复指定名称的会话：

$ abduco -c mysession

4. 设置会话标志：

$ abduco -r S mysession

5. 在新的会话中运行指定的程序：

$ abduco mysession -e top

上述是 abduco 命令的一些基本用法和示例，用户可以根据自己的需要选择不同的选项和参数来实现不同的功能。 

## tldr 
 
> 终端会话管理器。
> 更多信息：<http://www.brain-dump.org/projects/abduco/>.

- 列出会话：

`abduco`

- 附加到一个会话，如果不存在则新建它：

`abduco -A {{会话名}} {{终端}}`

- 使用`dvtm`附加到一个会话，如果不存在则新建它：

`abduco -A {{会话名}}`

- 从一个会话中分离：

`Ctrl + \`

- 以只读模式附加到一个会话：

`abduco -Ar {{会话名}}`
