# expand 
## chatgpt 
expand命令用于将tab转换为空格，将文件中的所有制表符替换为相应数量的空格。它可以将制表符替换为空格，也可以将空格替换为tab键，并且可以指定空格和tab替换的数量。

具体用法如下：

```sh
expand [选项] [文件名]
```

常见选项如下：

- -t n：将tab键转换为n个空格，默认为8个空格。
- -i：只将开头的空格或tab键转换为对应数量的另一种字符（空格或tab），而保留文件中其他位置的空格或tab键原样。
- -8：与-t 8相同，可用于显示制表符对应多少个空格。

例如，将tab键转换为空格：

```sh
expand file.txt
```

将tab键转换为4个空格：

```sh
expand -t 4 file.txt
```

将空格转换为tab键：

```sh
expand -t 4 -i file.txt
``` 

## tldr 
 
> 解压一个或多个 cab 文件。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/expand>.

- 将单文件 cab 文件解压到指定目录：

`expand {{cab 文件路径}} {{指定的目录}}`

- 列出 cab 文件中的所有文件：

`expand {{cab 文件路径}} {{指定的目录}} -d`

- 从 cab 文件中解压所有的文件：

`expand {{cab 文件路径}} {{指定的目录}} -f:*`

- 从 cab 文件中解压一个特定的文件：

`expand {{cab 文件路径}} {{指定的目录}} -f:{{文件名}}`

- 解压缩时忽略目录结构，并将它们添加到单个目录中：

`expand {{cab 文件路径}} {{指定的目录}} -i`
