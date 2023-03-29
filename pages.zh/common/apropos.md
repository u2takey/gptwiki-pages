# apropos 
## chatgpt 
apropos是一个Linux命令，它用于在系统的帮助文档中搜索与参数匹配的关键字或短语。 

具体来说，apropos命令将在Linux帮助文档（man pages）的描述部分中查找和参数相关的字符串。这些man pages通常包括命令的功能、语法、选项和示例等详细信息。

例如，要查找有关“network”的所有Linux命令，可以在终端中输入以下命令：

```
apropos network
```

结果将显示所有包含“network”关键字的man pages。

除了在终端中使用，apropos命令还可用于嵌入Shell脚本或其他系统自动化任务中，以便在操作执行期间提供信息和帮助。 

## tldr 
 
> 在 manpages 中搜索，例如查找一个新命令。
> 更多信息：<https://manned.org/apropos>.

- 搜索关键字：

`apropos {{正则表达式}}`

- 搜索时不限制输出到终端宽度：

`apropos -l {{正则表达式}}`
