# date 
## chatgpt 
date 命令用于输出或设置当前系统的日期和时间。在不加参数的情况下，date 命令将显示当前日期和时间。

命令语法：`date [OPTION]... [+FORMAT]` 

常见的选项包括：

- `-s or --set`: 设置系统时间。后面必须加上时间字符串，例如：`date -s "2021-09-12 15:30:00"`
- `-u or --utc`: 显示或设置为 UTC 时间，即格林威治标准时间。
- `-R or --rfc-2822`: 显示时间格式为 RFC-2822 标准格式。
- `-I or --iso-8601`: 显示时间格式为 ISO 8601 标准格式。例如：`2021-09-12T15:30:00+08:00`
- `+%FORMAT`: 根据指定的格式输出日期和时间，其中 %FORMAT 是可选的参数，表示输出的时间格式，例如：`date +%Y-%m-%d %H:%M:%S`

以下是一些常见的格式化选项：

- `%Y`: 年份（4位数字）
- `%m`: 月份（01-12）
- `%d`: 日（01-31）
- `%H`: 小时（00-23）
- `%M`: 分（00-59）
- `%S`: 秒（00-60）
- `%a`: 本地的缩写星期几名称（例如 Sun）
- `%A`: 本地的完整星期几名称（例如 Sunday）
- `%b`: 本地的缩写月份名称（例如 Jan）
- `%B`: 本地的完整月份名称（例如 January）
- `%z`: 时区偏移量（例如 +0800）

注意：date 命令执行需要管理员权限。 

## tldr 
 
> 设置或显示系统日期。
> 更多信息：<https://ss64.com/osx/date.html>.

- 使用默认区域设置的格式显示当前日期：

`date +"%c"`

- 以 UTC 和 ISO 8601 格式显示当前日期：

`date -u +"%Y-%m-%dT%H:%M:%SZ"`

- 将当前日期显示为 unix 时间戳（自 1970-01-01 00:00:00 以来的秒数）：

`date +%s`

- 使用默认格式显示特定日期（格式化指定 UNIX 时间戳）：

`date -r 1473305798`