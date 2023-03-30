# qlmanage 
## chatgpt 
qlmanage是macOS系统中的一个命令行工具，它允许用户快速查看、预览各种文件及其内容，而无需打开应用程序。以下是该命令的详细解释：

用法：qlmanage [选项] [文件名]

选项：

- -h：显示帮助信息。
- -m：启动沙盒模式。
- -p：预览指定文件，此选项需要结合文件路径一起使用。
- -t：测试指定文件有无预览功能，此选项需要结合文件路径一起使用。
- -x：运行指定文件的Quick Look扩展程序。
- -s：显示Quick Look服务器信息及属性。

使用qlmanage，您可以：

1. 预览文件：使用“-p”选项，qlmanage会在终端中显示指定文件的预览内容。例如，要预览名为“example.pdf”的PDF文件，可以输入以下命令：

   qlmanage -p example.pdf

该命令将显示PDF文件的预览内容。

2. 测试文件：使用“-t”选项，qlmanage可以测试指定的文件是否支持Quick Look功能。例如，要测试名为“example.docx”的Word文档是否支持Quick Look，可以输入以下命令：

   qlmanage -t example.docx

如果文件支持Quick Look，则会打印“quicklookd[pid] has registered new file”信息，否则将打印错误信息。

3. 运行Quick Look扩展程序：使用“-x”选项，qlmanage可以运行指定文件类型的Quick Look扩展程序。例如，要运行PDF文档的Quick Look扩展程序，可以输入以下命令：

   qlmanage -x com.apple.Preview example.pdf

该命令将启动“预览”的Quick Look扩展程序，并预览指定的PDF文件。

4. 显示Quick Look服务器信息及属性：使用“-s”选项，qlmanage可以显示Quick Look服务器的信息及属性，例如，当前Quick Look是否正在运行。例如，要查看Quick Look服务器的信息，可以输入以下命令：

   qlmanage -s

该命令将在终端中显示Quick Look服务器的信息及属性。

总之，qlmanage可以快速查看、测试和预览各种文件及其内容，是macOS系统中非常有用的命令行工具。 

## tldr 
 
> QuickLook 服务器工具。
> 更多信息：<https://ss64.com/osx/qlmanage.html>.

- 快速显示一个或多个文件：

`qlmanage -p {{文件名}} {{文件名 2}}`

- 计算生成当前目录中所有 jpeg 文件的缩略图，300px 宽 png 格式，并将它们放在一个指定目录中：

`qlmanage {{*.jpg}} -t -s {{300}} {{指定目录}}`

- 重置快速查看：

`qlmanage -r`
