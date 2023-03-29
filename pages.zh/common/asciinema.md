# asciinema 
## chatgpt 
asciinema 是一款基于终端的屏幕录制工具。它可以在终端中记录用户的操作，以 ASCII 录制，并且支持与 asciinema.org 网站的集成。通过 asciinema，用户可以将他们终端中的所有操作录制下来，包括输入、输出、命令、各种程序的运行情况等，然后将其分享给其他用户。

具体来讲，asciinema 的主要用法是：

1. 录制终端会话

使用 asciinema 记录命令行会话，可以通过以下命令来启动录制：

```
asciinema rec
```

录制完成后，asciinema 默认会将录制结果保存在本地磁盘上，可以用以下命令上传到 asciinema.org 网站分享：

```
asciinema upload <filename.cast>
```

2. 回放录制会话

asciinema 还支持播放录制会话，可以通过以下命令来回放录制的会话：

```
asciinema play <url>
```

比如回放 https://asciinema.org/a/113463 的录制：

```
asciinema play https://asciinema.org/a/113463
```

在播放过程中，用户可以调整播放速度、暂停或停止播放等。此外，asciinema 还提供了一些其他的命令和选项，可以通过以下命令来查看：

```
asciinema --help
``` 

## tldr 
 
> 录制和播放终端会话，也可以把他们分享到 asciinema.org.
> 更多信息：<https://asciinema.org/docs/usage>.

- 将本地安装的`asciinema`与 asciinema.org 账号关联：

`asciinema auth`

- 进行新的录制（完成后，将提示用户上传或在本地保存）：

`asciinema rec`

- 进行新的录制，保存到本地的文件中：

`asciinema rec {{文件路径}}.cast`

- 从本地文件中播放终端录屏：

`asciinema play {{文件路径}}.cast`

- 在 asciinema.org 中播放终端录屏：

`asciinema play https://asciinema.org/a/{{文件 ID}}`

- 进行新的录制，将闲置时间设置为最多 2.5 秒：

`asciinema rec -i {{2.5}}`

- 打印本地保存的录像的完整输出：

`asciinema cat {{文件路径}}.cast`

- 从本地上传一个录屏到 asciinema.org：

`asciinema upload {{文件路径}}.cast`
