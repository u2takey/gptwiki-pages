# gchown 
## chatgpt 
该命令是不存在的，可能是您需要使用的命令为 chown。 

chown 命令用于修改文件或目录的所有者和/或所属组。该命令需要 root 权限来运行。使用 chown 命令有两种方式，分别是使用用户 ID 和用户组 ID，或使用用户名和用户组名来指定：

使用用户 ID 和用户组 ID 指定：

```
chown [-R] <用户 ID>:<用户组 ID> <文件名/目录名>
```

例如，将文件 /var/www/html/index.html 的所有者修改为用户 ID 1001，所属组修改为用户组 ID 1005：

```
sudo chown 1001:1005 /var/www/html/index.html
```

使用用户名和用户组名指定：

```
chown [-R] <用户名>:<用户组名> <文件名/目录名>
```

例如，将文件 /var/www/html/index.html 的所有者修改为用户名 webuser，所属组修改为用户组名 webgroup：

```
sudo chown webuser:webgroup /var/www/html/index.html
```

使用 -R 选项可以递归修改一个目录及其子目录中的所有文件的所有者和/或所属组。例如：

```
sudo chown -R 1001:1005 /var/www/html/
```

这将递归修改目录 /var/www/html/ 及其子目录中的所有文件的所有者为用户 ID 1001，所属组为用户组 ID 1005。 

## tldr 
 
> 这是 `-p linux chown` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux chown`
