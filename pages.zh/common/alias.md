# alias 
## chatgpt 
alias命令用于为一个命令或一组命令创建一个别名，以便更方便地使用。它的一般语法为：

```bash
alias [alias-name[='command']]
```

其中，

- alias-name是您要为其创建别名的命令的名称。
- 如果不指定=command，shell将返回特定命令的别名列表。
- 如果您指定了=command，它将成为该命令的新别名。如果您在指定命令时使用空格和其他标点符号，请将它们放在引号中。

举个例子，如果您想为常用的 "ls -lh" 命令创建一个别名 "ll"，您可以这样做：

```bash
alias ll='ls -lh'
```

现在，每当您输入 "ll" 命令时，shell 将自动运行 "ls -lh" 命令。

您可以通过输入 "alias" 命令来列出所有别名。您也可以使用 "unalias" 命令来删除已创建的别名。 

## tldr 
 
> 创建别名 -- 用给定的字符串指代特定的命令。
> 别名只会在当前的 shell 会话中生效，除非它们在 shell 的配置文件中被定义，例如`~/.bashrc`.
> 更多信息：<https://tldp.org/LDP/abs/html/aliases.html>.

- 创建一个通用的别名：

`alias {{别名}}="{{命令}}"`

- 通过给定的别名查看它所指代的命令：

`alias {{别名}}`

- 移除一个别名：

`unalias {{别名}}`

- 列出所有的别名：

`alias -p`

- 将 rm 转换为交互式命令：

`alias {{rm}}="{{rm -i}}"`

- 创建别名 `la` 来指代 `ls -a`：

`alias {{la}}="{{ls -a}}"`
