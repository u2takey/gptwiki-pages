# megadl 
## chatgpt 
"megadl"是Linux系统中的一个命令。这个命令是一个Mega.nz的下载器，可以帮助用户从Mega.nz云存储平台下载文件。

具体使用方法：

1、安装megatools

在终端中输入以下命令即可安装megatools：

sudo apt-get install megatools

2、使用megadl下载文件

使用megadl下载Mega.nz上的文件，需要知道待下载的文件Mega链接，该链接是一个以“https://mega.nz/#!”开头的链接。在终端中输入以下命令即可:

megadl 'Mega链接'

“Mega链接”是待下载的文件的Mega链接。

例如：

如果想要下载链接为：https://mega.nz/#!AkxkzBLL!Lyow-kZOOJ1H7sRpMvCr-dWAnNlG5H-gX9xNqHPzJc8

则在终端中输入的命令为：

megadl 'https://mega.nz/#!AkxkzBLL!Lyow-kZOOJ1H7sRpMvCr-dWAnNlG5H-gX9xNqHPzJc8'

注意：如果不指定一个输出文件名，会使用默认的文件名作为输出文件名，例如下面的名称：

MEGA文件生成时间-文件名

例如：

MEGA2018-12-25_233815_test.jpg

这是因为 Megatools 程序添加了 timestamp。

3、其他常用选项

-v: 显示下载进度信息

--path：指定下载路径

-f：从文件读取Mega链接

例如，在终端中输入以下命令，可以将下载的文件存储在指定路径 /home/user/Documents 中：

megadl -v --path '/home/user/Documents' 'https://mega.nz/#!AkxkzBLL!Lyow-kZOOJ1H7sRpMvCr-dWAnNlG5H-gX9xNqHPzJc8' 

## tldr 
 
> 这是 `megatools-dl` 命令的一个别名。
> 更多信息：<https://megatools.megous.com/man/megatools-dl.html>.

- 原命令的文档在：

`tldr megatools-dl`
