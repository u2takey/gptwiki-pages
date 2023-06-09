# w 
## chatgpt 
w 命令用于显示当前系统活动的用户列表，包括他们所在的终端、登录时间、CPU 使用情况以及当前正在做的事情。

具体说明：
- 用户名：显示连接到系统的用户名
- 终端：显示连接到系统的终端名称
- 远程地址：如果是远程连接，则显示连接的 IP 地址
- 登录时间：显示用户开始登录系统的时间
- 闲置时间：显示用户上次输入命令到现在的时间
- JCPU：显示所有 shell 和进程使用的 CPU 时间总和
- PCPU：显示当前进程的 CPU 使用情况
- 命令：显示当前用户正在运行的命令或程序

使用语法：
```
w [选项]
```

常用选项：
- -h：以可读的方式输出时间
- -u：显示用户名和闲置时间
- -s：只显示登录时间、闲置时间和 JCPU
- -f：显示从 SysV 风格控制台连线的用户信息，该选项不能和 -u 同时使用
- -o：不显示标题行

示例：
```
w -h
w -u
w -f
``` 

## tldr 
 
> 显示登录者及其进程。
> 更多信息：<https://www.geeksforgeeks.org/w-command-in-linux-with-examples/>.

- 显示当前登录的所有用户的信息：

`w`

- 显示有关特定用户的信息：

`w {{用户}}`

- 显示信息而不包括标题：

`w --no-header`

- 显示信息不包括登录、JCPU 和 PCPU 列：

`w --short`
