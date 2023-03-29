# axel 
## chatgpt 
axel是一个Linux和Unix操作系统环境下的多线程下载工具，在终端环境下使用。

命令格式：

axel [选项] [URL]

常用选项：

- -n: 指定下载线程数，默认为2
- -s: 指定下载的分段大小，默认为10MB
- -o: 指定下载文件的名称或路径
- -v: 显示详细的下载过程信息
- -q: 静默模式，只输出关键信息
- -k: 重新开启下载时跳过已经下载完成的部分
- -c: 断点续传，从上次下载中断处开始下载

使用示例：

1. 下载文件：

axel http://example.com/example.file

2. 指定下载线程数和下载分段大小：

axel -n 4 -s 20M http://example.com/example.file

3. 指定下载文件名称或路径：

axel -o /home/user/downloads/example.file http://example.com/example.file

4. 断点续传下载：

axel -c http://example.com/example.file

5. 查看下载详细信息：

axel -v http://example.com/example.file

6. 静默模式下载：

axel -q http://example.com/example.file

注意事项：

1. 在某些情况下，axel可能会由于网站反爬取措施而无法下载文件。
2. 下载速度受网络连接和文件服务器带宽影响，不一定能达到最大速度。 

## tldr 
 
> 一款下载加速器。
> 支持 HTTP、HTTPS 和 FTP.
> 更多信息：<https://github.com/axel-download-accelerator/axel>.

- 链接下载：

`axel {{超链接}}`

- 链接下载，指定文件名：

`axel {{超链接}} -o {{文件名称}}`

- 多连接数下载：

`axel -n {{连接数量}} {{超链接}}`

- 查询镜像：

`axel -S {{镜像数量}} {{超链接}}`

- 限制下载速度（字节 bite 每秒）：

`axel -s {{字节数}} {{超链接}}`
