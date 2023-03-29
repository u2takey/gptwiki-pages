# mpv 
## chatgpt 
mpv 是一个基于命令行的多媒体播放器，支持各种音频和视频格式。以下是 mpv 命令的详细解释：

语法: mpv [选项] [URL|FILE|打开方式]

选项:
  -h, --help                          显示帮助信息
  -v, --version                       显示版本信息
  --no-config                         禁用配置文件
  --no-quiet                          不静默运行
  --msg-level <level>                 确定输出级别 (详细见下)
      --force-window=<yes|no|auto>    强制使用窗口
  --ontop                             设置窗口置顶或取消置顶
  --wid=<wid>                         使用指定的窗口 ID
  --input-ipc-server=<filename>       指定使用的 IPC 服务器
  --input-ipc-client=<filename>       指定 IPC 客户端文件
  --fullscreen                       设置全屏模式 (默认)
  --no-fullscreen                    关闭全屏模式
  --fs                               等同于 --fullscreen
  --fs-screen=<n>                    指定显示器编号
  --keep-open                        播放完文件后不退出
  --no-video                         禁用视频
  --no-audio                         禁用音频
  --audio-file=<file>                指定音频文件
  --audio-device=<device>            指定音频设备
  --gapless-audio                    允许无缝音频转换
  --no-gapless-audio                 禁用无缝音频转换
  --audio-buffer=<size>              设置音频缓冲区大小
  --audio-channels=<n>               设置音频通道数
  --audio-format=<fmt>               指定音频格式
  --audio-samplerate=<rate>          设置音频采样率
  --monitorpixelaspect=<ratio>       设置像素宽高比
  --window-scale=<x>/<y>             设置窗口缩放比例
  --force-window-position=<x> <y>    强制设置窗口位置
  --geometry=<w>x<h>+<x>+<y>         以指定尺寸和位置打开窗口
  --border                           加载带边框的窗口界面

URL|FILE|打开方式:
  要播放的视频或音频文件的路径，或者一个 URL。具体支持格式可在帮助信息中查看。

示例:
  mpv video.mp4                      播放视频文件
  mpv https://youtu.be/wvCGX9Nq3Uk  播放 YouTube 视频
  mpv --fs screen://0                在第一个显示器全屏播放
  mpv --audio-device=alsa:pcm=hw.1   播放指定的音频设备 

## tldr 
 
> 一个基于 MPlayer 的音频/视频播放器。
> 更多信息：<https://mpv.io>.

- 播放一个音频或视频文件：

`mpv {{文件名}}`

- 往后/往前 跳跃 5 秒：

`LEFT <or> RIGHT`

- 往后/往前 跳跃一分钟：

`DOWN <or> UP`

- 减少/增加 10% 播放速度：

`[ <or> ]`

- 以指定速度播放文件（0.01 到 100, 默认是 1）：

`mpv --speed {{速度}} {{文件名}}`

- 用 `mpv.conf` 中指定的一个用户配制播放文件：

`mpv --profile {{配制名称}} {{文件名}}`

- 播放摄像头或其他设备的输出：

`mpv /dev/{{video0}}`
