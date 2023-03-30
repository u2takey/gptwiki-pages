# mkdir 
## chatgpt 
mkdir是英文"make directory"的缩写，它是一个在Linux和其他Unix系统中常用的命令，用于创建一个新的空目录。

语法：
```
mkdir [选项] 目录名
```

常用选项：

- -m, --mode=模式
  指定目录的权限模式，例如：mkdir -m 755 mydir 表示创建一个名为mydir的目录，并赋予755的访问权限。

- -p, --parents
  递归创建目录。例如：mkdir -p a/b/c/d 表示创建a目录，并在a目录中依次创建b、c、d目录。

- -v, --verbose
  输出详细信息。例如：mkdir -v mydir 表示创建一个名为mydir的目录，并输出详细信息。

示例：

- 创建一个名为mydir的目录：
```
mkdir mydir
```

- 递归创建一个名为a/b/c/d的目录：
```
mkdir -p a/b/c/d
```

- 创建一个名为mydir的目录，并赋予777的访问权限：
```
mkdir -m 777 mydir
```

- 创建一个名为mydir的目录，并输出详细信息：
```
mkdir -v mydir
``` 

## tldr 
 
> 创建一个目录。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/mkdir>.

- 创建一个目录：

`mkdir {{目录名}}`

- 递归创建目录及子目录：

`mkdir {{子目录名}}`
