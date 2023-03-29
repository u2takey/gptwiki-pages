# cat 
## chatgpt 
cat 命令常用于连接并显示文件内容，其英文全称为“concatenate”，意思是“连接”。该命令可以用于以下操作：

1. 显示文件内容：如果不加任何参数，cat 命令将打开一个文件并显示它的内容。

2. 连接多个文件：使用 cat 命令可以将多个文件连接在一起，形成一个新文件。例如，以下命令可以将 file1、file2 和 file3 文件内容连接到一个名为 newfile 的新文件中：

   cat file1 file2 file3 > newfile

3. 重定向文件内容：可以使用 cat 命令将文件内容重定向到其他文件中。例如，以下命令可以将 file1 文件内容复制到 file2 文件中：

   cat file1 > file2

4. 显示行号：使用 cat 命令的 -n 选项可以显示每一行的行号。例如，以下命令将在显示文件内容的同时显示行号：

   cat -n file

5. 合并文件：通过 cat 命令可以将多个文件合并成一个。例如，以下命令将 file1 和 file2 文件合并成一个文件 newfile：

   cat file1 file2 > newfile

总之，cat 命令的主要功能是显示或连接文件内容。 

## tldr 
 
> 打印和拼接文件的工具。
> 更多信息：<https://www.gnu.org/software/coreutils/cat>.

- 以标准输出，打印文件内容：

`cat {{file}}`

- 多文件合并到目标文件：

`cat {{file1}} {{file2}} > {{target_file}}`

- 多文件合并，并追加到目标文件：

`cat {{file1}} {{file2}} >> {{target_file}}`

- 显示行号：

`cat -n {{file}}`

- 显示不可打印和空白的字符（使用 `M-` 前缀标记非 ASCII 字符）：

`cat -v -t -e {{file}}`
