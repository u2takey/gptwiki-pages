# fc-list 
## chatgpt 
命令: fc-list

fc-list命令用于列出系统上已安装的所有字体。它使用Fontconfig库来查找字体，并列出所有可用的字体系列和样式。 Fontconfig库是一个用于管理系统字体的库，可以控制应用程序使用哪些字体。

该命令可以按字体系列、字体格式、字体权重等分类来显示字体。

使用该命令时，也可以指定字体的详细信息，如代码点、规范化名称、可读名称、字体文件名、字体文件格式等。

语法：

`fc-list [选项] [模式]`

选项：

- `-f(--format)`：指定输出格式
- `-h(--help)`：显示帮助信息
- `-v(--version)`：显示版本信息
- `-q(--quiet)`：静默模式，不输出任何信息

模式：

- `pattern`：指定要匹配的字体模式，可以包含字体系列、字体格式、字体权重等信息

示例：

1. 列出所有安装的字体

```
fc-list
```

2. 列出安装的所有TrueType字体

```
fc-list : family format==TrueType
```

3. 列出安装的所有Sans字体

```
fc-list : family==Sans
```

4. 指定输出格式，仅输出字体名称

```
fc-list -f "%{family}\n"
``` 

## tldr 
 
> 列出系统上安装的可用字体。
> 更多信息：<https://manned.org/fc-list>.

- 返回系统中已安装字体的列表：

`fc-list`

- 返回具有给定名称的已安装字体的列表：

`fc-list | grep '{{DejaVu Serif}}'`

- 返回系统中已安装字体的数量：

`fc-list | wc -l`
