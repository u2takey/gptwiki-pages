# type 
## chatgpt 
type命令用于显示指定命令的类型。当我们在终端上输入一个命令时，我们可能不知道它是一个系统内置的命令还是一个外部程序或是一个脚本文件，使用type命令可以将其类型确定。

语法：

```
type [options] [command]
```

其中，command是要查询的具体命令。

常用选项：

- -t或--type：仅输出命令类型；
- -p或--path：仅输出命令路径；
- -a或--all：输出所有匹配命令并按顺序排列；
- --help：显示帮助文档。

举例说明：

1. 查看ls命令类型

```
$ type ls
ls is aliased to `ls --color=auto'
```

从输出结果可以看出，我们定义了一个别名，将ls命令替换为了`ls --color=auto`。这里的类型是alias(别名）。

2. 查看cd命令类型

```
$ type cd
cd is a shell builtin
```

从输出结果可以看出，cd是内部程序，它是shell的内置命令。这里的类型是shell builtin(内部程序）。

3. 查看java命令类型

```
$ type java
java is /usr/bin/java
```

从输出结果可以看出，java是外部程序，它的完整路径为/usr/bin/java。这里的类型是/usr/bin/java(外部程序)。

总之，type命令是一个简单但十分有用的命令，可以帮助我们确定一个命令的具体类型。 

## tldr 
 
> 显示文件的内容。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/type>.

- 显示特定文件的内容：

`type {{文件的路径}}`
