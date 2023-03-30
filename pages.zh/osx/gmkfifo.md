# gmkfifo 
## chatgpt 
gmkfifo是一个Linux命令，用于创建FIFO（First In, First Out）管道文件。FIFO管道文件是用于进程间通信的一种特殊文件类型。与管道不同的是，FIFO管道文件可以在磁盘上保存，并且可以被多个进程读写。

具体用法是：gmkfifo [文件名]

例如，以下命令将创建一个名为“myfifo”的FIFO管道文件：

gmkfifo myfifo

该命令将在当前目录下创建一个名为“myfifo”的文件，这个文件用于进程间通信。文件创建后，可以使用其他命令（如cat和echo）将数据写入到该文件或从该文件中读取数据。

需要注意的是，FIFO不像普通的文件，不会自己删除，必须手动删除。可以使用rm命令来删除FIFO文件。 

## tldr 
 
> 这是 `-p linux mkfifo` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux mkfifo`
