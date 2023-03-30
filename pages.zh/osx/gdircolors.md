# gdircolors 
## chatgpt 
gdircolors是一个Linux命令，用于生成和打印GNU ls颜色方案。 

GNU ls是列出目录内容的标准命令，在默认情况下ls命令显示的文件或目录都是黑白的，为了更好的区分文件或目录，ls命令提供了一种彩色显示的选项，在不同的操作系统或Linux发行版中，GNU ls有不同的默认颜色方案。 

gdircolors的作用就是生成和打印GNU ls颜色方案。 

gdircolors命令的常用选项包括： 

- --help：显示帮助信息
- --version：显示命令版本号
- --print-database：打印系统默认的颜色方案
- -p：打印生成的颜色方案
- -b：以bash shell脚本的格式输出颜色方案

用法示例：

生成和打印默认的GNU ls颜色方案：gdircolors

生成和打印新的GNU ls颜色方案：gdircolors > ~/.dir_colors

查看生成的颜色方案：more ~/.dir_colors

使用新的颜色方案：eval "$(gdircolors -q ~/.dir_colors)" 

## tldr 
 
> 这是 `-p linux dircolors` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux dircolors`
