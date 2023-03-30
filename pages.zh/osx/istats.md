# istats 
## chatgpt 
iStats是一个可以监控Mac电脑硬件信息的命令行工具，包括CPU、GPU、硬盘、电池、传感器等，可以实时了解电脑的状态。

该命令的使用方式如下：

`istats [选项] [参数]`

其中，选项可以是：

- `--all`：显示所有可用传感器信息。
- `--cpu`：显示CPU相关的信息。
- `--gpu`：显示GPU相关的信息。
- `--battery`：显示电池相关的信息。
- `--fan`：显示风扇相关的信息。
- `--disk`：显示硬盘相关的信息。
- `--memory`：显示内存相关的信息。
- `--help`：显示命令帮助信息。

参数可以是：

- `--value-numeric`：以数字方式显示数值。
- `--value-short`：以短文本方式显示数值。
- `--no-labels`：不显示标签（例如：温度、频率）。
- `--no-graphs`：不显示图表。

例如，要显示CPU温度和频率的信息，可以使用以下命令：

`istats --cpu`

如果需要以数字方式显示数值，可以在后面加上参数`--value-numeric`：

`istats --cpu --value-numeric`

除此之外，还可以通过`watch`命令实现实时监控电脑状态：

`watch -n 1 istats`

这个命令表示每隔1秒钟运行一次`istats`命令，实时展示电脑状态。 

## tldr 
 
> 一个显示 CPU 温度、风扇速度和电池状态等统计数据的命令行工具。
> 更多信息：<https://github.com/Chris911/iStats>.

- 显示所有的统计数据：

`istats`

- 显示所有 CPU 的统计数据：

`istats cpu`

- 显示所有风扇的统计数据：

`istats fan`

- 扫描和打印温度：

`istats scan`
