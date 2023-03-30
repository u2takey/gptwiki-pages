# xed 
## chatgpt 
命令：xed

命令描述：xed是GNU / Linux操作系统中的一种文本编辑器，它可用于在命令行界面中编辑文本文件。

语法：xed [ OPTIONS ] [ FILE ]

选项：

- -V，--version：显示xed的版本信息。
- -h，--help：显示xed的帮助信息。
- -g，--geometry=GEOMETRY：设置xed的窗口大小和位置。
- -s，--start=NUMBER：设置打开文件时滚动窗口的起点（行号）。
- -w，--wrap=MODE：设置行的折行模式，可选“none”，“word”或“char”。
- -b，--background-color=COLOR：设置xed窗口的背景颜色。
- -f，--font=FONT：设置xed窗口中文本的字体。
- -l，--line-numbers：在左侧显示行号。
- -i，--insert-spaces：在缩进时使用空格而不是制表符。
- -a，--autosave-interval=SECONDS：设置自动保存的时间间隔（秒）。
- -c，--color-theme=THEME：选择xed的颜色主题。

示例：

1. 打开文件：

	xed myfile.txt

2. 设置字体和背景颜色：

	xed -f "DejaVu Sans Mono 10" -b "#181818" myfile.txt

3. 显示行号和使用空格缩进：

	xed -l -i myfile.txt

4. 设置颜色主题：

	xed -c "Monokai" myfile.txt

5. 设置折行模式：

	xed -w "word" myfile.txt

6. 设置自动保存时间间隔：

	xed -a 60 myfile.txt 

## tldr 
 
> 用 Xcode 打开要编辑的文件。
> 更多信息：<https://www.manpagez.com/man/1/xed/>.

- 用 Xcode 打开文件：

`xed {{文件名}}`

- 在 Xcode 中打开文件，如果不存在则创建：

`xed -c {{文件名}}`

- 在 Xcode 中打开一个文件并跳转到第 75 行：

`xed -l 75 {{文件名}}`
