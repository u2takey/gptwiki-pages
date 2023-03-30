# fc 
## chatgpt 
fc命令是Linux和Unix操作系统中的一个命令，用于比较和编辑制定的两个文件或者历史命令。该命令可以用于以下几个方面：

1. 比较两个文本文件的内容并显示差异：
fc file1 file2

2. 编辑上一条命令：
fc

3. 编辑历史记录中某个命令：
fc -e -5

其中，-e选项表示直接在编辑器中打开历史命令，-5表示编辑倒数第5条命令。

4. 编辑历史记录中两个命令之间的所有命令：
fc -s 100 110

以上命令将打开编辑器并显示编号为100到110之间的所有历史记录命令。

5. 撤销最近的命令并重新执行编辑后的命令：
fc -s

6. 批量重复执行某个命令：
fc -r

以上是fc命令的一些常见用法和选项，可以根据具体的需求进行灵活运用。 

## tldr 
 
> 比较两个文件或文件集之间的差异。
> 使用通配符（*）来比较文件集。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/fc>.

- 比较两个指定的文件：

`fc {{文件 1 的路径}} {{文件 2 的路径}}`

- 比较时不区分大小写：

`fc /c {{文件 1 的路径}} {{文件 2 的路径}}`

- 将文件作为 Unicode 文本来进行比较：

`fc /u {{文件 1 的路径}} {{文件 2 的路径}}`

- 将文件作为 ASCII 文本来进行比较：

`fc /l {{文件 1 的路径}} {{文件 2 的路径}}`

- 将文件作为二进制来比较：

`fc /b {{文件 1 的路径}} {{文件 2 的路径}}`

- 禁用制表符到空格的扩展：

`fc /t {{文件 1 的路径}} {{文件 2 的路径}}`

- 压缩空格（制表符和空格）进行比较：

`fc /w {{文件 1 的路径}} {{文件 2 的路径}}`