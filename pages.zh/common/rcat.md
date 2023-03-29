# rcat 
## chatgpt 
rcat是Remote Cat的缩写，它是一个基于SSH的远程文件复制工具。

命令语法：

rcat [-E] [-fnNdNiiprsSvVX] [-c cipher] [-e escapechar] [-k password | -i identity] [-o options] [-P port] [-T timeout] [-t targetuser] [-w password] [-x debugfile] [-z compression] [file | -] [user@]host:[directory/][file]

参数说明：

-E          保持环境变量  
-f          阻止远程的stdin输入到本地的stdout里  
-n          不进行压缩，即不再"netcat基础上增加的rcat传输特有的压缩算法"  
-N          不对输出进行转义  
-d          调试模式  
-i 【path】  使用identity 验证身份
-c          加密算法  
-e 【char】  逃脱字符，比如\e表示一个反斜杠，类似于echo命令的解释  
-k 【path】  使用password验证身份  
-o          SSH选项  
-P 【port】  SSH端口号  
-r          输出文件并且不删除它  
-s          打印目标机hostname和ssh版本信息  
-S 【path】  指定密钥文件路径  
-t 【user】  远程登录的用户  
-T 【sec】   连接超时时间  
-v          查看详细信息  
-X          显示调试信息  
-z 【algo】 压缩算法：zlib, lzo, none, auto（默认）  
- 【path】   发送标准输入到远程的命令行  
【user@】host 键入要连接的远程主机   

示例：

通过rcat将本地文件上传至远程主机：

rcat file.txt user@example.com:/path/to/remote/directory/

使用rcat将远程主机的文件下载到本地：

rcat user@example.com:/path/to/remote/file.txt - > local-file.txt 

通过管道将本地数据上传到远程主机：

echo "Hello World" | rcat - user@example.com:/path/to/remote/file.txt

查看rcat版本信息：

rcat -v 

## tldr 
 
> 这是 `rc` 命令的一个别名。

- 原命令的文档在：

`tldr rc`
