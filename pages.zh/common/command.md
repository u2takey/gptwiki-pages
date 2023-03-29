# command 
## chatgpt 
`command` 是一个 shell 内置命令，用于执行指定命令并覆盖当前 shell 环境的功能。

命令语法：

```
command [-pVv] command [arguments ...]
```

参数说明：

- `-p`：输出执行命令时使用的 PATH 环境变量。如果没有指定执行命令，则输出当前 PATH 环境变量。
- `-V`：显示执行命令的版本信息。
- `-v`：显示执行命令时使用的命令名称。

示例：

1. 显示当前 shell 使用的 PATH 环境变量：

```
$ command -p
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
```

2. 查看执行命令的版本信息：

```
$ command -V ls
ls --color=auto
```

3. 查看执行命令时的命令名称：

```
$ command -v ls
ls
```

4. 将指定命令添加到默认的 PATH 环境变量中：

```
$ command -p export PATH=$PATH:/usr/local/mysql/bin
```

注意事项：

- 如果执行命令为 shell 关键字，如 `cd`、`echo` 等，`command` 不会影响命令执行。
- 如果执行命令为 shell 函数，则可以使用 `command` 命令将其覆盖后执行。 

## tldr 
 
> Command 强制当前 shell 执行指定程序，并忽略具有相同名称的任何函数、内置函数和别名。
> 更多信息：<https://manned.org/command>.

- 从字面上执行 `ls` 程序，即使存在 `ls` 别名：

`command {{ls}}`

- 显示指定命令的可执行程序路径或别名定义：

`command -v {{命令名}}`
