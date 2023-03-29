# carbon-now 
## chatgpt 
carbon-now是一个命令行工具，用于快速创建代码截图，并将其分享到carbon.now.sh网站。

其详细解释如下：

1. 安装carbon-now

运行以下命令来安装carbon-now：

```
npm install --global carbon-now-cli
```

2. 运行carbon-now

在终端中输入以下命令来运行carbon-now：

```
carbon-now [options] [file]
```

其中，file是要截图的代码文件的路径。

3. 选项

carbon-now支持以下选项：

- --bg、-b：指定背景颜色。例如：--bg "#2e2e2e"。
- --config、-c：指定配置文件的路径。
- --copy、-y：将截图复制到剪贴板上。
- --crop、-o：裁剪截图以适应代码的长度。
- --current、-cd：使用当前目录作为代码文件的路径。
- --debug、-d：打印调试信息。
- --fontSize、-fs：指定字体大小。例如：--fontSize 14。
- --help、-h：打印帮助。
- --lineNumbers、-l：启用行号。
- --padding、-p：指定内边距。例如：--padding 32。
- --theme、-t：指定代码编辑器的主题。例如：--theme visor。

4. 截图内容

carbon-now默认截图包含以下内容：

- 代码文件名
- 代码编辑器的主题
- 代码编辑器的语言
- 代码行数
- 单行代码的长度
- 代码文件的内容

5. 截图分享

carbon-now默认将截图上传到carbon.now.sh网站，并返回截图的URL。您可以使用这个URL来分享截图。 

## tldr 
 
> 创建漂亮的代码图片。
> 更多信息：<https://github.com/mixn/carbon-now-cli>.

- 使用默认设置从文件创建图片：

`carbon-now {{文件}}`

- 使用默认设置从剪贴板创建图片：

`carbon-now --from-clipboard`

- 使用默认设置从标准输入创建图片：

`{{输入}} | carbon-now`

- 以交互方式创建图片以进行自定义设置，还可以选择保存预设：

`carbon-now -i {{文件}}`

- 从先前保存的预设创建图片：

`carbon-now -p {{预设}} {{文件}}`

- 从指定的文本行开始：

`carbon-now -s {{行号}} {{文件}}`

- 结束于指定的文本行：

`carbon-now -e {{行号}} {{文件}}`

- 在浏览器中打开图片而不是保存：

`carbon-now --open {{文件}}`
