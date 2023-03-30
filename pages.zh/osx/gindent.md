# gindent 
## chatgpt 
"gindent"命令是GNU Indent这个程序的两种形式之一（另一个是"indent"）。GNU Indent是一个用于缩排C代码的程序，可以根据用户指定的选项在源代码中添加缩进、空格、换行等控制符号。这有助于提高代码的可读性和可维护性。

"gindent"命令的使用方式与"indent"命令基本相同，可以通过命令行参数来控制缩进的风格、缩进的层数、空格的数量等。例如，使用"gindent -kr -ts4 myfile.c"命令可以将"myfile.c"文件中的代码以K&R风格缩进，缩进层数为4，每级缩进使用4个空格。

除了命令行参数外，gindent也支持配置文件来指定缩进的样式，例如"/usr/share/indent/default.st"就是gindent默认的配置文件。在配置文件中，用户可以设置一系列参数，包括注释的位置、空格的长度、缩进的数量、换行的方式等。

需要注意的是，gindent只能处理合法的C代码文件，并且会直接修改文件内容。因此，在进行缩排操作之前，最好备份一下源代码文件。 

## tldr 
 
> 这是 `-p linux indent` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux indent`
