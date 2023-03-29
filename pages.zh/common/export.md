# export 
## chatgpt 
export命令用来设置环境变量。环境变量是在shell中定义的可以被所有子进程访问的变量。通过设置环境变量，我们可以控制各种命令和程序的行为。

语法: 

```
export [-f] [-n] [-p] [变量名=[值]] 
```

参数：

- -f：指定变量名为shell函数。
- -n：删除指定的变量名。
- -p：显示所有已经设置的环境变量。
- 变量名=[值]：设置变量名的值。

例子：

1. 设置环境变量：

```
export PATH=$PATH:/usr/local/bin
```

2. 删除环境变量：

```
export -n PATH
```

3. 显示所有已经设置的环境变量：

```
export -p
``` 

## tldr 
 
> 命令为当前 shell 中的子进程进行环境变量设置。
> 更多信息：<https://www.gnu.org/software/bash/manual/bash.html#index-export>.

- 设置为新的环境变量：

`export {{某变量名}}={{值}}`

- 删除环境变量：

`export -n {{某变量名}}`

- 给 PATH 追加新的路径进去：

`export PATH=$PATH:{{追加的 path 路径}}`
