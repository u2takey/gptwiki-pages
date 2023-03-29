# arecored 
## chatgpt 
很抱歉，作为AI语言模型，我必须指出“arecored”不是一个有效的Linux命令。但是，基于推测，可能是“arecord”这个命令，下面是对该命令的详细解释：

arecord是ALSASoundCardRecordingUtility的缩写。它是alsa-utils软件包中的一部分，允许在Linux中录制音频。

具体来说，arecord命令允许在Linux中捕捉音频流（如麦克风或耳机），并将其保存为.wav或其他格式的文件。该命令可以用于进行音频记录或创建自定义音频应用程序。

以下是arecord命令的常见选项：

- -f：指定音频数据的格式（如pcm、s8、s16等）
- -D：选择要捕获的声卡设备
- -d：指定录制的持续时间（以秒为单位）
- -r：指定采样率（例如，44100表示44.1 kHz采样率）
- -c：指定记录的通道数（1表示单声道、2表示立体声）

以下是arecord命令的示例：

1. 捕捉通过麦克风的音频，并将其保存为“recording.wav”文件：

    $ arecord -f cd -d 60 -t wav -D default recording.wav

2. 将立体声音频流保存到“recording.wav”文件中：

    $ arecord -f dat -c 2 -r 44100 -d 10 recording.wav

请注意，在运行arecord命令之前，您需要了解有关声卡设备、采样率、录制时间和文件格式等方面的信息。 

## tldr 
 
> ALSA 声卡驱动的声音录制器。
> 更多信息：<https://manned.org/arecord>.

- 以 "CD" 质量录制一段声音（录制结束以 Ctrl-C 停止）：

`arecord -vv --format=cd {{路径/文件名.wav}}`

- 以 "CD" 质量录制 10 秒钟声音：

`arecord -vv --format=cd --duration={{10}} {{路径/文件名.wav}}`

- 录制一段声音并以 mp3 格式保存（录制结束以 Ctrl-C 停止）：

`arecord -vv --format=cd --file-type raw | lame -r - {{路径/文件名.mp3}}`

- 列出所有的声卡和数字音频设备：

`arecord --list-devices`

- 允许交互式界面（例如使用空格键或回车键来播放或暂停）：

`arecord --interactive`
