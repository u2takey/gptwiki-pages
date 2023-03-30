# afinfo 
## chatgpt 
afinfo是macOS系统上的一个命令行工具，用于获取音频文件的信息。它可以提供音频文件的格式、时长、比特率、采样率、通道数等信息。

afinfo命令的使用方法如下：

```bash
afinfo [音频文件路径]
```

其中，音频文件路径是指要获取信息的音频文件的绝对路径或相对路径。

举个例子，如果要获取一个名为music.mp3的音频文件的信息，可以使用以下命令：

```bash
afinfo /Users/username/Music/music.mp3
```

此时，afinfo将输出音频文件的信息，示例如下：

```bash
File:           /Users/username/Music/music.mp3
File type ID:   MPG3
Num Tracks:     1
----
Data format:     2 ch,  44100 Hz, 'lpcm' (0x0000000C) 16-bit big-endian signed integer
estimated duration: 202.134286 sec
----
Data format:     2 ch,  44100 Hz, 'mp3 ' (0x00000000) 0 bits/channel, 0 bytes/packet, 1152 frames/packet, 0 bytes/frame
estimated duration: 202.134286 sec
``` 

其中，可以看到音频文件的格式为MPG3，通道数为2，采样率为44100 Hz，时长为202.134286秒。同时，afinfo还提供了音频文件的原始格式（lpcm）信息以及MP3格式信息。 

## tldr 
 
> 显示音频文件元数据（Metadata）详细信息（OS X）。
> OS X 自带命令。
> 更多信息：<https://ss64.com/osx/afinfo.html>.

- 显示给定音频文件的详细信息：

`afinfo {{目标 / 路径 / 文件}}`

- 显示简化的音频文件信息（单行）：

`afinfo -b {{目标 / 路径 / 文件}}`

- 显示音频文件的元数据信息以及其 InfoDictionary 词典：

`afinfo -i {{目标 / 路径 / 文件}}`

- 以 xml 格式显示音频文件信息：

`afinfo -x {{目标 / 路径 / 文件}}`

- 显示警告信息（如存在）：

`afinfo --warnings {{目标 / 路径 / 文件}}`

- 显示完整用法帮助：

`afinfo -h`
