# ack 
## chatgpt 
命令 "ack" 是一个命令行工具，用于在给定的文件和目录中搜索文本。"ack" 可以在文本文件、代码文件、配置文件和其他文本文件中查找文本。

以下是使用 "ack" 命令的常见选项：

1. `-i`：忽略大小写进行匹配。
2. `-w`：仅匹配完整单词。
3. `-l`：仅打印文件名而不显示文件中匹配到的文本。
4. `-c`：仅打印匹配的行数，而不打印匹配的文本。
5. `-n`：在匹配的行之前打印行号。
6. `-v`：只显示没有匹配到的行。

例如，要在当前目录中搜索包含字符串 "Apple" 的文件，可以使用以下命令：

```
ack "Apple"
```

要在搜索中忽略大小写，可以添加 `-i` 选项：

```
ack -i "apple"
```

要在搜索中仅显示文件名，可以添加 `-l` 选项：

```
ack -l "Apple"
```

要在搜索中添加行号，可以添加 `-n` 选项：

```
ack -n "Apple"
``` 

## tldr 
 
> 一个类似 grep 的搜索工具，为程序员优化。
> 另见 `rg`，它要快得多。
> 更多信息：<https://beyondgrep.com/documentation>.

- 在当前目录下递归地搜索包含一个字符串或正则表达式的文件：

`ack "{{search_pattern}}"`

- 不区分大小写搜索：

`ack --ignore-case "{{search_pattern}}"`

- 搜索匹配模式的行，只打印匹配的文本，而不打印行的其他部分：

`ack -o "{{search_pattern}}"`

- 限制搜索特定类型的文件：

`ack --type={{ruby}} "{{search_pattern}}"`

- 不在特定类型的文件中搜索：

`ack --type=no{{ruby}} "{{search_pattern}}"`

- 计算找到的匹配文件的总数：

`ack --count --no-filename "{{search_pattern}}"`

- 只打印文件名和每个文件的匹配数：

`ack --count --files-with-matches "{{search_pattern}}"`

- 列出所有可与 `--type` 一起使用的值：

`ack --help-types`
