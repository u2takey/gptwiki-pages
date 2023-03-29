# afconvert 
## chatgpt 
afconvert 是 macOS系统下的一个命令行工具，用于音频格式转换和处理。

语法：

    afconvert [options] input_file output_file

参数：

- `input_file`：待转换的音频文件路径。
- `output_file`：转换后的音频文件路径。

选项：

- `-f FORMAT`：指定输出音频的格式，例如 `-f wav`,`-f mp3`等。
- `-d CODEC`：指定编码器，例如 `-d aac`，`-d wav`等。
- `-q QUALITY`：指定音频质量，例如 `-q 127`。
- `-b BITRATE`：指定比特率，例如 `-b 128k`。
- `-c CHANNELS`：指定声道数。
- `-s SAMPLE_RATE`：指定采样率。

其他常用选项：

- `-d LEI16@44100`：指定输出为16比特、小端模式、44100Hz采样率的线性PCM（常用）。
- `-d I8`：指定输出为8比特的整数PCM。
- `-d I16`：指定输出为16比特的整数PCM。
- `-d I24`：指定输出为24比特的整数PCM。
- `-d F32`：指定输出为32比特的浮点PCM。
- `-d MP3`：指定输出为MP3格式。
- `-d AAC`：指定输出为AAC格式。
- `-d AIFF`：指定输出为AIFF格式。
- `-d WAVE`：指定输出为WAV格式。
- `-d CAF`：指定输出为CAF格式。

示例：

1. 将 `inputfile.wav` 转换为 `outputfile.aac`，比特率为128k，采样率为44100Hz：

    ```
    afconvert -f m4af -d aac -b 128000 -s 44100 inputfile.wav outputfile.aac
    ```

2. 将 `inputfile.aiff` 转换为 `outputfile.mp3`，比特率为128k，声道数为2：

    ```
    afconvert -f mp4f -d mp3 -b 128000 -c 2 inputfile.aiff outputfile.mp3
    ```

3. 将 `inputfile.wav` 转换为 `outputfile.flac`，无损压缩：

    ```
    afconvert -f flac -d flac inputfile.wav outputfile.flac
    ``` 

## tldr 
 
> 在 AFF 和 raw 文件格式之间进行转换。
> 更多信息: <https://manned.org/afconvert.1>.

- 使用一个特定的扩展名（默认：`aff`）：

`afconvert -a {{扩展名}} {{路径/到/输入文件}} {{路径/到/输出文件1 路径/到/输出文件2 ...}}`

- 使用一个特定的压缩级别（默认：`7`）：

`afconvert -X{{0..7}} {{路径/到/输入文件}} {{路径/到/输出文件1 路径/到/输出文件2 ...}}`
