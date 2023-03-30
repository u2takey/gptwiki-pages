# gmktemp 
## chatgpt 
gmktemp 是一个生成临时文件或目录的命令。利用该命令可以快速地在文件或目录中创建临时文件或目录，这些文件或目录可用于临时存储数据或者执行一些操作。其具体用法如下：

1. 生成临时文件：gmktemp file

file 是指生成临时文件的前缀，gmktemp 命令会在该前缀后面添加一些随机字符来生成一个唯一的文件名。例如：

$ gmktemp file
/tmp/file.za8Wb

2. 生成临时目录：gmktemp -d directory

directory 是指生成临时目录的前缀，gmktemp 命令会在该前缀后面添加一些随机字符来生成一个唯一的目录名。例如：

$ gmktemp -d directory
/tmp/directory.9zfN9

3. 生成多个临时文件：gmktemp -t file1 file2 file3...

-t 参数表示生成多个临时文件，后面跟上需要生成的临时文件前缀。例如：

$ gmktemp -t file1 file2 file3
/tmp/file1.ZLDxw /tmp/file2.OS2Qr /tmp/file3.HX9sm

当然，gmktemp 命令还有其他一些参数，可以通过 man gmktemp 命令来查看其完整的用法说明。 

## tldr 
 
> 这是 `-p linux mktemp` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux mktemp`
