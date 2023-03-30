# taskkill 
## chatgpt 
Taskkill是一个Windows操作系统的命令行工具，用于终止一个或多个进程。

语法：

taskkill [/s Computer] [/u Domain\User [/p Password]]] [{/fi Filter}] [/im ImageName [/f]] [/pid ProcessID] [/t]

参数：

/s 选项用于指定要在其上终止进程的远程计算机。

/u 选项用于指定用于在远程计算机上执行任务终止操作的凭据。

/p 选项用于指定密码。

/fi 选项用于过滤要终止的进程。

/im 选项用于指定要终止的映像名称。

/pid 选项用于指定要终止的进程ID。

/t 选项用于终止进程树。

示例：

1. 停止名称为notepad.exe的进程。

taskkill /im notepad.exe

2. 终止指定进程ID为1234的进程。

taskkill /pid 1234

3. 终止名称为notepad.exe和calc.exe的进程。

taskkill /im notepad.exe /im calc.exe

4. 终止进程树。

taskkill /pid 1234 /t

注意：

使用Taskkill命令时，请注意不要意外终止其他正在运行的程序，否则可能会导致数据损坏或系统出现错误。 

## tldr 
 
> 按进程 id 或进程名终止进程。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/taskkill>.

- 通过进程 id 终止进程：

`taskkill /pid {{进程 id}}`

- 通过进程名终止进程：

`taskkill /im {{进程名}}`

- 强制终止一个指定的进程：

`taskkill /pid {{进程名}} /f`

- 终止一个进程及其子进程：

`taskkill /im {{进程名}} /t`

- 终止远程计算机上的进程：

`taskkill /pid {{进程 id}} /s {{远程主机名}}`

- 显示命令的帮助信息：

`taskkill /?`
