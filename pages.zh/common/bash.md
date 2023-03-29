# bash 
## chatgpt 
bash是Linux中一种常用的shell（命令行解释器）。 

使用bash命令可以打开一个Bash Shell，也就是一个交互式的命令行终端。 

在Bash Shell中，可以执行各种命令，如文件操作、目录操作、网络操作等等。也可以通过Bash脚本编写一系列命令，批量处理某些工作或命令的输出结果。 

常用的bash命令包括：

- cd：进入到指定的目录；
- ls：显示指定目录中的文件和子目录；
- mkdir：创建一个新的目录；
- rm：删除一个文件或目录；
- mv：移动或重命名文件或目录；
- cp：复制文件或目录；
- grep：在文件中查找文本；
- echo：在终端上打印输出；
- cat：连接文件并显示输出；
- chmod：修改文件或目录的访问权限；
- passwd：修改当前用户的密码等等。

总之，bash是处理Linux系统上的各种命令和任务的核心组件之一。 

## tldr 
 
> Bourne-Again SHell.
> 兼容`sh`的命令行解释器。
> 更多信息：<https://gnu.org/software/bash/>.

- 启动交互式 shell：

`bash`

- 执行命令：

`bash -c "{{command}}"`

- 执行脚本文件：

`bash {{file.sh}}`

- 执行脚本文件，并将所有执行过的命令输出到终端：

`bash -x {{file.sh}}`

- 执行脚本文件，并在第一个错误处终止：

`bash -e {{file.sh}}`

- 从输入（stdin）读取命令：

`bash -s`

- 将跟随的所有选项原样传递到要执行的脚本文件（可与`-s`选项共用来将选项传递到来自输入的命令 / 脚本）：

`bash --`

- 打印 bash 的版本信息（使用`echo $BASH_VERSION`来获得纯粹的版本字符串）：

`bash --version`
