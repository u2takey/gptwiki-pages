# bmaptool 
## chatgpt 
bmaptool是一个用于创建和写入Block Map映像文件的命令行工具，通常用于在烧录树莓派等嵌入式设备镜像时优化磁盘写入效率。Block map是一种描述运行操作系统或其他软件程序的映像模式的文件格式。使用该文件格式，可以跳过为写入空闲数据而进行的不必要操作，仅写入映像数据中使用的块，从而减少磁盘上的写入操作次数，提高写入效率。

bmaptool具有以下常用选项：

- create：创建Block Map映像文件。
- copy：将映像文件数据复制到目标设备上。
- info：显示映像文件的元数据信息。
- stats：显示映像文件的统计信息。
- verify：验证映像文件和目标设备之间的数据一致性。
- compare：比较两个映像文件之间的数据。
- read：从映像文件读取数据并输出到标准输出。
- write：将数据写入映像文件。

使用bmaptool可以提高烧录镜像时的效率，尤其是在复制大文件时。 

## tldr 
 
> 便捷地创建或复制块文件映射（被设计的比`cp`或`dd`更快）。
> 更多信息：<https://source.tizen.org/documentation/reference/bmaptool>.

- 使用图片生成块图文件：

`bmaptool create -o {{blockmap 格式文件.bmap}} {{图片文件}}`

- 复制图片到指定目录：

`bmaptool copy --bmap {{blockmap 格式文件}} {{图片文件}} {{/开发路径/sdb}}`

- 复制压缩后的图片到指定目录：

`bmaptool copy --bmap {{blockmap 格式文件}} {{图片文件.gz}} {{/开发路径/sdb}}`

- 复制图片的时候，不将图片转成块图：

`bmaptool copy --nobmap {{图片文件}} {{/开发路径/sdb}}`
