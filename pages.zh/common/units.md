# units 
## chatgpt 
命令 "units" 是一个可以用于转换单位的命令行工具。它可以将一个物理量从一个单位转换到另一个单位。该命令的基本使用方法如下：

1. 打开终端或命令行窗口；
2. 输入 "units" 命令；
3. 输入要转换的物理量及其单位，比如 "10cm"；
4. 输入目标单位，比如 "inches"。

此时，命令行界面将返回转换后的结果，例如 "3.9370079 inches"。

除了基本用法，"units" 命令还支持以下高级功能：

1. 支持不同的输出格式，包括分式、指数、浮点数等；
2. 可以进行复合单位的转换，比如将 "pound force per square inch" 转换为 "joule per cubic meter"；
3. 可以利用配置文件进行自定义单位的定义和转换。

总之，"units" 命令是一个非常强大而又简单易用的单位转换工具，可以在科学、工程、计算等领域广泛应用。 

## tldr 
 
> 提供两个度量单位之间的转换。
> 更多信息：<https://www.gnu.org/software/units/>.

- 以交互模式运行：

`units`

- 显示两个简单单位之间的转换：

`units {{quarts(夸脱)}} {{tablespoons(大汤匙)}}`

- 单位与数量之间的转换：

`units "{{15 pounds(磅)}}" {{kilograms(公斤)}}`

- 显示两个复合单位之间的转换：

`units "{{meters(米) / second(秒)}}" "{{inches(英尺) / hour(小时)}}"`

- 显示具有不同维度的单位之间的转换：

`units "{{acres(英亩)}}" "{{ft(英尺)^2(平方)}}"`

- 显示字节乘数的转换：

`units "{{15 megabytes(兆字节)}}" {{bytes(字节)}}`
