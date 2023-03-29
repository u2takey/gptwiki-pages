# mkdir 
## chatgpt 
mkdir是Linux/Unix系统中的一个命令，用于创建一个新目录或目录树。

命令格式为：

```
mkdir [选项] 目录名
```

常用选项说明：

- -p：递归创建目录。如果目录已经存在，则不会出错，也不会进行任何操作。
- -m：指定目录权限。需要在后面加上所要设置的权限值，比如777。
- -v：显示创建过程。

例如，执行以下命令：

```
mkdir -p /home/userA/example
```

将会创建一个名为example的目录，它将被放在/home/userA/目录下。如果/home/userA/目录不存在，则也将被创建。

执行以下命令：

```
mkdir -m 777 /home/userA/example
```

将会创建一个名为example的目录，它将被放在/home/userA/目录下，并且其权限将被设置为777（即所有用户都具有读、写、执行权限）。

执行以下命令：

```
mkdir -v /home/userA/example
```

将会创建一个名为example的目录，并在创建过程中显示详细信息。例如，“mkdir: created directory '/home/userA/example'”就是一条创建结果的输出。 

## tldr 
 
> 创建目录。
> 更多信息：<https://www.gnu.org/software/coreutils/mkdir>.

- 在当前目录或给定路径下创建一个目录：

`mkdir {{目录}}`

- 在当前目录下创建多个目录：

`mkdir {{目录_1 目录_2 ...}}`

- 递归地创建目录（对创建嵌套目录很有用）：

`mkdir -p {{路径/到/目录}}`
