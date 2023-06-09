# stat 
## chatgpt 
命令名称：stat

命令功能：显示文件或文件系统的状态信息

命令参数：

-a或--all：除了.和..之外，同时也列出所有文件

-c或--format：根据指定的格式输出状态信息

-f：显示文件系统状态而非文件状态

--help：显示帮助信息

-L或--dereference：对于拥有符号链接的文件，显示其链接指向的文件状态而非链接文件本身状态

-t或--terse：简明模式，仅输出文件或文件系统状态信息的第一行

--version：显示版本信息

命令示例：

1. 显示文件的状态信息

$ stat file.txt

输出结果类似于：

文件：‘file.txt’

大小： 1024 字节

块大小： 4096 字节

设备： 804h/2052d Inode： 262329 硬链接： 1

访问：（0644/-rw-r--r--） Uid： (1000/ bob) Gid： (1000/ bob)

最近访问： 2021-10-01 14:41:51.216121838 +0800

最近更改： 2021-10-01 14:41:51.216121838 +0800

最近的文件状态更改： 2021-10-01 14:41:51.216121838+0800

创建时间：-

2. 显示目录的状态信息

$ stat dir

输出结果类似于：

文件：‘dir’

大小： 4096个块

块大小： 4096字节

设备： 804h/2052d Inode： 393271 硬链接： 2

访问：（0755/drwxr-xr-x） Uid： (1000/ bob) Gid： (1000/ bob)

最近访问： 2021-10-01 14:41:51.188121946 +0800

最近更改： 2021-10-01 14:35:27.428114680 +0800

最近的文件状态更改： 2021-10-01 14:35:27.428114680 +0800

创建时间： -

3. 显示文件系统的状态信息

$ stat -f /

输出结果类似于：

文件： “/”

ID： b92f407e-1956-4d19-a582-986901af5c5e

块大小： 4096 字节

总块数： 999798734

剩余块数： 996364215

可用块数： 936020833

Inodes 总数： 254279936

可用 Inodes： 253690268

所有者： root：根

群组： root

类型： ext4

装载点： /

4. 显示文件的状态信息，仅输出第一行

$ stat -t file.txt

输出结果类似于：

file.txt 1024 4096 -rw-r--r-- 1000 1000 262329 1- 1633077711 1633077711 1633077711 0 

## tldr 
 
> 显示文件状态。
> 更多信息：<https://ss64.com/osx/stat.html>.

- 显示文件属性，如大小、权限、创建和访问日期等：

`stat {{文件}}`

- 与上面相同，但更详细（更类似于 Linux 的 `stat`）：

`stat -x {{文件}}`

- 只显示文件权限：

`stat -f %Mp%Lp {{文件}}`

- 显示文件的所有者和所属组：

`stat -f "%Su %Sg" {{文件}}`

- 以字节为单位显示文件的大小：

`stat -f "%z %N" {{文件}}`
