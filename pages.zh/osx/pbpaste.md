# pbpaste 
## chatgpt 
pbpaste是一个macOS和iOS系统中的命令行工具，它用于将剪贴板中的内容输出到终端（或者直接使用管道将其输出到另一个命令）。以下是pbpaste命令的用法和示例：

用法：

pbpaste [-help]

示例：

1. 将剪贴板中的文本粘贴到终端：

    pbpaste

2. 将剪贴板中的文本输出到一个新的文本文件中：

    pbpaste > new_file.txt

3. 将剪贴板中的内容输出到另一个命令中：

    pbpaste | grep "search_string"

在以上示例中，pbpaste命令简单而且易于使用，它非常适合需要从剪贴板中复制文本并将其粘贴到终端中的场景。 

## tldr 
 
> 将剪贴板的内容发送到标准输出（命令行）。
> 更多信息：<https://ss64.com/osx/pbpaste.html>.

- 将剪贴板的内容写入文件：

`pbpaste > {{文件}}`

- 将剪贴板的内容用作命令的输入：

`pbpaste | grep foo`
