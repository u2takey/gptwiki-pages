# wget 
## chatgpt 
wget命令是一个非常强大的命令行工具，用于从Web服务器下载文件。wget命令支持HTTP、HTTPS和FTP协议，支持通过代理服务器下载文件。

以下是wget命令的一些常用选项和参数：

- -O：指定下载文件的名称（如果不指定将使用默认名称）。
- -c：支持断点续传，如果下载过程中中断，再次执行wget命令时会从断点处继续下载。
- -r：递归下载，下载指定URL中的所有链接。
- -np：不下载父级目录，通常与-r选项一起使用。
- -nH：不创建主机名目录，通常与-r选项一起使用。
- -nd：不创建目录结构，所有下载的文件将放在当前目录下。

以下是一些wget命令的示例：

1. 下载单个文件：

```
wget https://example.com/file.zip
```

2. 下载文件并重命名：

```
wget -O newfile.zip https://example.com/file.zip
```

3. 断点续传：

```
wget -c https://example.com/largefile.zip
```

4. 递归下载：

```
wget -r https://example.com/
```

5. 不下载父级目录：

```
wget -r -np https://example.com/
```

6. 不创建主机名目录：

```
wget -r -nH https://example.com/
```

7. 不创建目录结构：

```
wget -r -nd https://example.com/
```

wget命令可以大大简化文件下载过程，但请注意下载的文件是否合法和版权问题。 

## tldr 
 
> 从网络上下载文件。
> 支持 HTTP, HTTPS, 和 FTP.
> 更多信息：<https://www.gnu.org/software/wget>.

- 将该 URL 的内容下载到文件中（在这个例子中文件名为 "foo"）：

`wget {{https://example.com/foo}}`

- 将该 URL 的内容下载到文件中（在这个例子中文件名为 "bar"）：

`wget --output-document {{bar}} {{https://example.com/foo}}`

- 以每三秒一个请求的速度下载一个网页和其所有资源（脚本，样式表，图片等等）：

`wget --page-requisites --convert-links --wait=3 {{https://example.com/somepage.html}}`

- 从一个目录中下载所有列出的文件和其所有子文件夹（不下载内嵌网页）：

`wget --mirror --no-parent {{https://example.com/somepath/}}`

- 限制下载速度和重试次数：

`wget --limit-rate={{300k}} --tries={{100}} {{https://example.com/somepath/}}`

- 使用基本授权来从 HTTP/FTP 服务器中下载文件：

`wget --user={{username}} --password={{password}} {{https://example.com}}`

- 继续一个未完成的下载任务：

`wget --continue {{https://example.com}}`

- 将指定文件中所有列出的 URL 下载到一个目录中：

`wget --directory-prefix {{path/to/directory}} --input-file {{URLs.txt}}`
