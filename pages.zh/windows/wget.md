# wget 
## chatgpt 
wget是一个命令行工具，可以在Linux和Unix系统上使用。它用于从Web服务器下载文件或整个网站。它可以下载HTTP，HTTPS和FTP协议下的文件。

wget命令常用的参数：

- `-O`: 指定下载的文件名。
- `-q`: 静默模式，不输出过程信息。
- `-c`: 断点续传，遇到网络中断时重新下载文件。
- `-r`: 递归下载，下载完整个网站。
- `-nH`: 不创建主机目录，将下载的文件直接存放在当前目录下。

举个例子，假设我们要从https://example.com/index.html下载文件，我们可以使用以下命令：

```
wget https://example.com/index.html
```

如果我们要将下载的文件重命名为new_index.html，我们可以用-O参数来实现：

```
wget -O new_index.html https://example.com/index.html
```

如果我们要下载整个网站，我们可以使用-r参数：

```
wget -r https://example.com/
```

这将下载example.com域下的所有文件，包括图片、CSS文件等。这个命令可能会花费很长时间，因此建议使用-c参数以便重新下载中断的文件。 

## tldr 
 
> 这是 `wget -p common` 命令的一个别名。
> 更多信息：<https://www.gnu.org/software/wget>.

- 原命令的文档在：

`tldr wget -p common`
