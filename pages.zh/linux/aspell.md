# aspell 
## chatgpt 
aspell是一个用于拼写检查和字典管理的命令行工具。

aspell命令的基本语法如下：

```
aspell [options] [file1] [file2] ...
```

参数说明：

- `[options]`：可选参数，用于设置aspell的行为。常见的选项包括：
  - `-c`：检查拼写并显示建议纠正方式。
  - `-a`：检查拼写并显示所有可用的建议纠正。
  - `-l <lang>`：指定要使用的语言。
  - `-t`：将每个拼写错误显示为其文本周围的上下文。
- `[file1] [file2] ...`：可选参数，指定要检查拼写的文件路径。如果未给出文件路径，则aspell默认从标准输入流中读取输入。

使用aspell检查拼写的示例命令：

```
aspell -c readme.txt
```

此命令将检查readme.txt文件中的拼写，并列出所有拼写错误及其建议的修正方式。

要查看aspell支持的所有选项，请运行以下命令：

```
aspell --help
``` 

## tldr 
 
> 交互式拼写检查工具。
> 更多信息：<http://aspell.net/>.

- 为一个文件做拼写检查：

`aspell check {{文件路径}}`

- 列出来自标准输入的拼写错误单词：

`cat {{文件}} | aspell list`

- 列出可用的字典语言：

`aspell dicts`

- 指定不同的语言（取 ISO 639 语言代码的 2 个字母）来运行 `aspell`：

`aspell --lang={{cs}}`

- 列出来自标准输入的拼写错误单词，并且忽略个人单词列表中的单词：

`cat {{文件}} | aspell --personal={{个人单词列表.pws}} list`
