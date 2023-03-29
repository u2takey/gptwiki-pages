# aplay 
## chatgpt 
aplay命令是一个用于在Linux系统上播放alsa声音文件的命令。它是alsa-utils包中的一部分，通常已预装在许多Linux发行版中。

aplay命令可以使用以下语法：

aplay [options] [filename]

其中filename是要播放的声音文件的名称或路径。如果未指定文件名，则aplay将等待从标准输入中读取数据。

以下是一些常用选项:

- -c, --channels: 指定声道数。
- -f, --format：指定声音文件的格式。
- -D, --device：指定要使用的声音设备。
- -v, --verbose：显示详细信息。

示例：

1. 播放WAV文件:

aplay example.wav

2. 使用16位的PCM格式播放文件:

aplay -f S16_LE example.wav

3. 播放立体声文件:

aplay -c 2 example.wav

4. 在常规输出中显示有关播放状态的详细信息：

aplay -v example.wav 

## tldr 
 
> ALSA 声卡驱动程序的命令行声音播放器。
> 更多信息：<https://manned.org/aplay>.

- 播放一个文件（会自动根据文件格式确定采样率、位深等）：

`aplay {{文件路径}}`

- 以 2500 Hz 播放指定文件的前 10 秒：

`aplay --duration={{10}} --rate={{2500}} {{文件路径}}`

- 以 22050 Hz，mono，8-bit，Mu-Law 和 `.au` 格式来播放指定原始文件：

`aplay --channels={{1}} --file-type {{raw}} --rate={{22050}} --format={{mu_law}} {{文件路径}}`
