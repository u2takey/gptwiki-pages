# bpytop 
## chatgpt 
bpytop 是一款用 Python 编写的基于终端的系统资源监控工具。它可以显示实时 CPU、内存、磁盘、网络等性能统计信息，并提供多种颜色方案和自定义设置选项。

首先，要在 Linux 终端中运行 bpytop，需要先在系统中安装 Python 和 pip 包管理器。可以通过以下命令安装 Python 和 pip：

```
sudo apt install python3-pip
```

安装完毕后，使用 pip 命令安装 bpytop：

```
pip3 install bpytop
```

安装完成后，可以直接在终端中运行 bpytop：

```
bpytop
```

bpytop 的界面分为多个部分，包括 CPU 使用率、内存使用情况、磁盘使用状态、网络流量监控等。可以通过上下箭头和回车键来选择不同的选项，例如选择不同的 CPU 核心、调整 CPU 刷新频率等。

另外，bpytop 还支持多种命令行参数和自定义配置选项，例如可以使用 `-t` 参数来指定刷新时间间隔，使用 `-C` 参数来选择不同的颜色方案等。

总的来说，bpytop 是一款功能强大、易于使用的系统资源监控工具，可以帮助用户实时了解系统的性能情况。 

## tldr 
 
> 用图形显示有关正在运行的进程的动态实时信息。类似于 `gtop` 和 `htop`.
> 更多信息：<https://github.com/aristocratos/bpytop>.

- 运行 bpytop：

`bpytop`

- 以最小模式启动，无需内存和网络盒：

`bpytop -m`

- 显示版本：

`bpytop -v`

- 切换最小模式：

`m`

- 搜索正在运行的程序或进程：

`f`

- 改变设置：

`M`
