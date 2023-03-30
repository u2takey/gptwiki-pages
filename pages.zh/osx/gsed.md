# gsed 
## chatgpt 
gsed是GNU版本的sed命令，它是用于在Unix和类Unix操作系统中编辑文本文件的流编辑器。 

gsed命令具有以下常用功能：
1.替换功能（s命令）：gsed可以使用s命令替换文本中的某个字符串。例如，gsed 's/old/new/g' file.txt将替换文件file.txt中的所有old为new。 
2.删除行/删除行范围（d命令）：gsed可以使用d命令删除行或范围中的行。例如，gsed '2d' file.txt将删除文件file.txt中的第二行。gsed '2,5d' file.txt将删除文件file.txt中的第二到第五行。 
3.添加行（a命令）：gsed可以使用a命令在指定行之后添加新行。例如，gsed '2a This is a new line' file.txt将在文件file.txt的第二行之后添加一行“This is a new line”。 
4.插入行（i命令）：zsed可以使用i命令在指定行之前插入一行。例如，gsed '2i This is a new line' file.txt将在文件file.txt的第二行之前插入一行“This is a new line”。 
5.打印文本（p命令）：gsed可以使用p命令打印文本中的某些行。例如，gsed -n '2p' file.txt将打印文件file.txt中的第二行。 

总之，gsed是一个强大而灵活的文本编辑器，可以用于从文本中提取信息、修改文件内容、格式化文本以及执行其他文本处理任务。 

## tldr 
 
> 这是 `-p linux sed` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sed`
