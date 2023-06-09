# gmknod 
## chatgpt 
gmknod命令用于在Linux操作系统（包括常见的发行版如Ubuntu、Debian、CentOS等）中创建块设备或字符设备节点文件。块设备通常用于存储设备，如硬盘、U盘等，而字符设备则通常用于I/O设备，如键盘、鼠标、打印机等。

该命令主要需要以下参数：

- -m：设置节点的访问权限；
- -n：设置节点的名称；
- -t：指定节点的类型，可选项为b（块设备）或c（字符设备）；
- major：设置块设备或字符设备的主设备号；
- minor：设置块设备或字符设备的次设备号。

例如，以下命令将创建一个名为mydev的块设备节点文件，该文件的主设备号为8，次设备号为1：

```
sudo gmknod -m 666 /dev/mydev b 8 1
```

需要注意的是，创建设备节点需要root权限。在创建设备节点时应小心，不要错误地使用复制、移动、删除等操作，并且应避免在系统根目录下创建设备节点。 

## tldr 
 
> 这是 `-p linux mknod` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux mknod`
