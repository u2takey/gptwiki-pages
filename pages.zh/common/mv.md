# mv 
## chatgpt 
命令mv用于将文件或目录移动到另一个位置或者重命名，其基本语法如下：

mv [OPTIONS] source destination

其中，OPTIONS为可选参数，source为源文件或源目录的路径，destination为目标文件或目标目录的路径。

移动文件或目录：

如果destination是一个目录，则会将source移动到该目录下。例如：

mv file.txt newdir/

将文件file.txt移动到目录newdir下。

如果destination为一个不存在的目录或文件，则会将source重命名为destination。例如：

mv oldfile.txt newfile.txt

将oldfile.txt重命名为newfile.txt。

重命名文件或目录：

在命令中只需要指定要重命名的源文件或目录，以及目标名称即可将其重命名：

mv oldfile.txt newfile.txt

将oldfile.txt重命名为newfile.txt。

例如：

mv olddir newdir

将目录olddir重命名为newdir。

值得注意的是，如果destination已经存在，则会覆盖已有的文件或目录。如果想要保留已存在的文件而同时将源文件或目录重命名，则需要使用-i选项：

mv -i oldfile.txt newfile.txt

这会在覆盖文件时提供提示。 

## tldr 
 
> 移动或重命名文件或目录。
> 更多信息：<https://www.gnu.org/software/coreutils/mv>.

- 移动文件到任意位置：

`mv {{来源}} {{目标}}`

- 移动文件到其他目录，并保持文件名不变：

`mv {{来源1}} {{来源2}} {{来源3}} {{目标目录}}`

- 覆盖现有文件前无需确认：

`mv -f {{来源}} {{目标}}`

- 无论是否有文件权限，覆盖现有文件前均需要确认：

`mv -i {{来源}} {{目标}}`

- 不要覆盖现有的目标文件：

`mv -n {{来源}} {{目标}}`

- 详细模式，移动后打印文件名：

`mv -v {{来源}} {{目标}}`
