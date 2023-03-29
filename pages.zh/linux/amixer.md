# amixer 
## chatgpt 
amixer 是 Linux 中的音频控制器，它允许用户控制音量、音频通道、麦克风等。amixer 命令可以用于调整系统音量、音频设备的输入和输出以及设备的状态。它还允许用户查询音频设备是否支持某些功能，以及设置音频设备参数，如音调、音效等。amixer 命令还可以用于设置音频设备的混合器，以允许用户在不同的音频设备之间切换。

以下是 amixer 命令的常见用法及相应的参数：

1. 查询系统音频设置：

amixer

2. 改变 PCM 的音量：

amixer set PCM <value>

value 的大小范围是 0 到 100。

3. 通过音频卡控制音量，与 PCM 不同：

amixer set Master <value>

4. 设定麦克风的音量：

amixer set Mic <value>

5. 设定耳机的音量：

amixer set Headphone <value>

6. 设定 Master 的音量：

amixer -c 0 set Master <value>

-c 选项表示是第一个音频卡。

7. 显示音频控制器的信息：

amixer info

8. 将音频设置存入文件中：

amixer -c 0 -p save > /etc/asound.state

将设置保存在 /etc/asound.state 文件中。

9. 从文件中读取音频设置：

amixer -c 0 -p restore < /etc/asound.state

从 /etc/asound.state 文件中读取设置。 

## tldr 
 
> ALSA 声卡驱动程序的混合器。
> 更多信息：<https://manned.org/amixer>.

- 增加 10% 的主音量：

`amixer -D pulse sset Master {{10%+}}`

- 降低 10% 的主音量：

`amixer -D pulse sset Master {{10%-}}`
