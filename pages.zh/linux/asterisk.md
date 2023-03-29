# asterisk 
## chatgpt 
在 Linux 命令行中，asterisk 是一个代表星号（*）的特殊符号。 

asterisk 可以用于多种用途，以下是几个示例： 

1. 使用通配符搜索文件 

在 Linux 中，可以使用通配符来匹配一组文件名。例如，如果要查找以 .txt 结尾的所有文件，可以使用以下命令：

```
$ ls *.txt
```

这个命令将列出当前目录下所有以 .txt 结尾的文件。在这里，* 就是代表所有的通配符。

2. 替换字符串 

另一个常见的用途是在命令行中替换字符串。例如，如果要将文件中所有的 "foo" 替换为 "bar"，可以使用 sed 命令：

```
$ sed 's/foo/bar/g' file.txt
```

在这里，* 会匹配任意数量的字符，从而确保所有的 "foo" 都被替换。

3. 在正则表达式中使用 

在正则表达式中，* 代表前面的字符可以出现 0 次或多次。例如，如果要匹配任意数量的 a，可以使用以下正则表达式：

```
a*
```

这将匹配 ""、"a"、"aa"、"aaa" 等任意数量的 a。

总之，asterisk 是一个非常有用的通配符和正则表达式标记，在 Linux 中的许多命令和操作中都可以使用。 

## tldr 
 
> 电话和交换（手机）服务器。
> 用于管理服务器自身和管理已经在运行的实例。
> 更多信息：<https://wiki.asterisk.org/wiki/display/AST/Home>.

- 重新连接一个正在运行的服务器，并打开 3 级的日志详细度：

`asterisk -r -vvv`

- 重新连接一个正在运行的服务器，执行一个命令，然后返回：

`asterisk -r -x "{{命令}}"`

- 显示 chan_SIP 客户端（手机）：

`asterisk -r -x "sip show peers"`

- 显示激活的通话和频道：

`asterisk -r -x "core show channels"`

- 显示语音邮箱：

`asterisk -r -x "voicemail show users"`

- 终止一个频道：

`asterisk -r -x "hangup request {{频道 ID}}"`

- 重新载入 chan_SIP 设置：

`asterisk -r -x "sip reload"`
