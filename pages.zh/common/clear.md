# clear 
## chatgpt 
命令“clear”用于清除终端或命令行窗口屏幕上的所有文本和输出。当您输入和执行一些命令并查看它们的输出后，终端窗口会变得杂乱无章。通过使用该命令，您可以轻松地将屏幕清空，重新开始执行新的命令或查看新的输出。 

该命令没有任何参数，只需在命令行中输入“clear”，然后按下“Enter”键即可。执行该命令时，所有当前屏幕上的内容都将被清除，您将看到一个空屏幕。需要注意的是，虽然执行该命令可以清除屏幕上的所有输出，但是当您向上滚动屏幕时，以前执行的命令的输出仍然存在，因此可以通过向上滚动屏幕查看以前输出的历史记录。 

## tldr 
 
> 清空终端的屏幕。
> 更多信息：<https://manned.org/clear>.

- 清空屏幕（相当于在 Bash shell 中按 Control-L 键）：

`clear`

- 清空屏幕但保留终端的回滚缓冲区：

`clear -x`

- 指明要清空的终端类型（默认为环境变量 `TERM` 的值）：

`clear -T {{type_of_terminal}}`

- 显示 `clear` 使用的 `ncurses` 版本：

`clear -V`
