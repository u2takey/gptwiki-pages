# basename 
## chatgpt 
basename命令用于去掉文件路径的目录部分，只返回文件名。其基本语法为：

`basename [string] [suffix]`

其中，string为要进行操作的字符串，可以是文件路径或纯文本字符串；suffix为可选参数，表示要去掉的后缀名。

例如，假设当前目录下有一个文件路径为`/root/path/filename.txt`，那么：

- `basename /root/path/filename.txt`将返回`filename.txt`
- `basename /root/path/filename.txt .txt`将返回`filename`

如果string为纯文本字符串，则不需要指定suffix参数。例如：

- `basename "hello world"`将返回`hello world`

使用basename命令时，需要注意以下几点：

1. basename命令只会去掉路径中的目录部分，并不会判断文件是否真的存在。
2. 如果不指定suffix参数，则basename命令会返回包含原始字符串的完整文件名。
3. 如果需要去掉多个后缀名，则需要连续调用多次basename命令。例如，`basename `basename filename.txt .txt``可以去掉两个后缀名。
4. basename命令也可以用于在shell脚本中获取当前脚本的文件名。例如，`basename $0`将返回当前脚本的文件名。 

## tldr 
 
> 移除一个路径的目录部分字符。
> 更多信息：<https://www.gnu.org/software/coreutils/basename>.

- 仅显示文件名：

`basename {{路径/到/文件}}`

- 显示路径字符最右边表示目录的字符：

`basename {{路径/到/目录/}}`

- 展示无后缀的文件名称：

`basename {{路径/到/文件}} {{后缀}}`
