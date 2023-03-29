# aria2c 
## chatgpt 
aria2c是一个命令行下载工具，可以通过多个协议（包括HTTP，FTP，BitTorrent等）下载文件。以下是该命令的详细说明：

用法：

`aria2c [选项] [URL | 文件]...`

选项：

- `-d, --dir=<目录>`：将下载的文件存储到指定目录，默认为当前目录。
- `-o, --out=<文件名>`：将下载的文件保存为指定文件名。
- `-s, --split=<数目>`：使用指定数目的连接进行下载。默认为5。
- `-x, --max-connection-per-server=<数目>`：在每个服务器上使用的最大连接数。默认为1。
- `-k, --min-split-size=<大小>`：最小分片大小。默认为20M。
- `-j, --max-concurrent-downloads=<数目>`：同时下载的最大文件数。默认为5。
- `-c, --continue`：继续未完成的下载任务。
- `-t, --timeout=<秒>`：设置超时时间，单位为秒。默认为60秒。
- `-m, --max-tries=<次数>`：设置最大重试次数。默认为5次。
- `-q, --quiet`：静默模式，不会输出任何信息。
- `--help`：显示帮助信息。
- `--version`：显示版本号。

示例：

下载单个文件：

`aria2c https://example.com/file.zip`

下载多个文件：

`aria2c https://example.com/file1.zip http://example.com/file2.zip`

使用指定的连接数进行下载：

`aria2c -s 10 https://example.com/file.zip`

将下载的文件保存到指定目录：

`aria2c -d /path/to/directory https://example.com/file.zip`

将下载的文件保存为指定文件名：

`aria2c -o myfile.zip https://example.com/file.zip`

继续未完成的下载任务：

`aria2c -c https://example.com/file.zip`

以上就是aria2c命令的详细说明。 

## tldr 
 
> 快速下载工具。
> 支持 HTTP(S), FTP, SFTP, BitTorrent, and Metalink.
> 更多信息：<https://aria2.github.io>.

- 下载一个 URI 到文件：

`aria2c {{url}}`

- 从多个源处下载一个资源：

`aria2c {{url_1}} {{url_2}}`

- 通过保存在一个文件中的 URL 列表来下载资源：

`aria2c -i {{文件名}}`

- 使用多个连接下载资源：

`aria2c -s {{连接数量}} {{url}}`

- 通过带用户名密码验证的 FTP 协议下载资源：

`aria2c --ftp-user={{用户名}} --ftp-passwd={{密码}} {{url}}`

- 限制下载速度（bytes/s）：

`aria2c --max-download-limit={{速度}} {{url}}`
