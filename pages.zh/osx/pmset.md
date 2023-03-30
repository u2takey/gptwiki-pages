# pmset 
## chatgpt 
pmset是一个用于管理和设置系统的电源管理设置的命令行工具。它可用于控制许多不同的电源选项，包括睡眠模式、显示设置、硬盘设置等等。以下是一些常用的命令：

1. pmset -g：列出当前系统所有的电源设置

2. pmset -a：更改所有电源选项

3. pmset -b：更改外部电源选项

4. pmset -c：更改电池选项

5. pmset -u：更改UPS选项

6. pmset -a sleep 10：将系统设置为在闲置10分钟后进入睡眠模式

7. pmset -c displaysleep 20：将外部电源选项设置为在20分钟的空闲时间后关闭屏幕。

8. pmset -b disksleep 30：将电池选项设置为在30分钟后关闭硬盘。

总的来说，pmset是一个非常有用的工具，可以帮助用户在不同的电源设置下优化电脑的电池寿命和性能。 

## tldr 
 
> 配置 macOS 电源管理设置，就像在系统首选项 > 节能程序中一样。
> 修改设置的命令必须以 `sudo` 开头。
> 更多信息：<https://ss64.com/osx/pmset.html>.

- 显示当前电源管理设置：

`pmset -g`

- 显示当前电源和电池电量：

`pmset -g batt`

- 立即让显示器进入休眠状态：

`pmset displaysleepnow`

- 当充电器通电时，将显示器设置为从不休眠：

`sudo pmset -c displaysleep 0`

- 使用电池电源 15 分钟后将显示器设置为休眠：

`sudo pmset -b displaysleep 15`

- 安排计算机在每个工作日上午 9 点自动唤醒：

`sudo pmset repeat wake MTWRF 09:00:00`

- 还原为系统默认值：

`sudo pmset -a displaysleep 10 disksleep 10 sleep 30 womp 1`
