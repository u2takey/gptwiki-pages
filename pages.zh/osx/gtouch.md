# gtouch 
## chatgpt 
gtouch是一个Linux/Unix命令，用于更新指定文件或目录的访问和修改时间戳。gtouch的工作原理是更新文件或目录的访问和修改时间戳，而不会更改文件的内容。

gtouch命令可以用以下方式使用：

```gtouch [选项]... [文件]...```
    
参数说明:
```
-f 不进行任何错误处理，仅使用正常的返回值，文件不存在时不会创建文件
-a 仅更新访问时间
-m 仅更新修改时间
-c 只有在要更新的文件存在时才更新时间戳
-t STAMP 通过指定的时间戳设置文件的记录时间
-r FILE 使用指定文件的时间戳信息更新指定文件的时间戳
--help 显示此帮助信息并退出
--version 显示版本信息并退出
```    
示例:

```gtouch test.txt``` 

以上命令会更新文件test.txt的访问和修改时间为当前时间。

```gtouch -m test.txt```

以上命令仅更新test.txt的修改时间戳，并保持访问时间戳不变。

```gtouch -a -t 201804251030 test.txt```

以上命令将文件test.txt的访问时间戳设置为2018年4月25日10:30。

希望以上解释可以帮到您。 

## tldr 
 
> 这是 `-p linux touch` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux touch`
