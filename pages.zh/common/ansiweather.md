# ansiweather 
## chatgpt 
命令：ansiweather 

该命令是一个用于获取天气信息的命令行工具，可以将所选地区的天气信息以 ANSI 转义序列的形式输出。该命令使用了 OpenWeatherMap API 来获取天气信息，需要有一个相关的 API 密钥才能使用。命令使用简单，可以通过指定城市名称、国家和地区代码、经纬度等参数来获取天气信息。无需浏览器或其他天气应用，即可通过命令行获取相关信息。

命令语法：

ansiweather [OPTIONS] [LOCATION]

LOCATION：地理位置，可以是城市名称，也可以是坐标。默认值是安装程序的本地位置。

OPTIONS：

-a ：显示所有数据

-u ：显示温度单位

-f ：指定从 OpenWeatherMap 获取天气信息时要使用的 API 密钥，即指定接口服务，并可在过期后重新生成。

-l ：使用本地时间而不是 UTC 时间

-p ：指定自定义格式，例如“\:%C\:%t\:%w\:%P\:%h”

-h, --help ：显示帮助信息

例子：
获取芝加哥的天气信息，使用摄氏度单位：

ansiweather -u metric Chicago

或使用经纬度获取西雅图的天气信息：

ansiweather -u metric -l 47.606,-122.33 

## tldr 
 
> 一个 shell 脚本，用于在终端中显示当前的天气状况。
> 更多信息：<https://github.com/fcambus/ansiweather>.

- 使用公制单位显示 Rzeszow, Poland 接下来 5 天的天气预报：

`ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}`

- 显示带符号和日光数据信息的天气预报：

`ansiweather -s {{true}} -d {{true}}`

- 显示带风力等级和湿度信息的天气预报：

`ansiweather -w {{true}} -h {{true}}`
