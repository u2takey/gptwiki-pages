# system_profiler 
## chatgpt 
system_profiler是macOS中的一个命令行工具，用于收集和报告有关系统硬件和软件配置的详细信息。该命令可以提供以下信息：

1.硬件信息：系统配置、处理器、内存、储存器、显示器、网络设备、输入设备等。

2.系统软件信息：操作系统版本、内核版本、引导设备、时间和日期等。

3.网络信息：网络配置、网络接口、路由器信息等。

4.程序信息：安装的应用程序和版本、已安装的字体等。

5.其他信息：系统日志、已连接的外围设备和 USB 设备信息。

该命令有多个参数，例如：

1. system_profiler -detaillevel full：输出详细硬件信息。

2. system_profiler -listDataTypes：返回可用的信息分类。

3. system_profiler SPNetworkDataType：输出网络相关信息。

使用该命令可以了解macOS系统的配置和硬件配置，方便硬件升级和系统配置问题的排查。 

## tldr 
 
> 报告系统硬件和软件配置。
> 更多信息：<https://ss64.com/osx/system_profiler.html>.

- 显示可由 System Profiler.app 打开的完整系统资源报告：

`system_profiler -xml > MyReport.spx`

- 显示硬件概述（型号、CPU、内存、串行等）：

`system_profiler SPHardwareDataType`

- 打印系统序列号：

`system_profiler SPHardwareDataType|grep "Serial Number (system)" |awk '{print $4}'`
