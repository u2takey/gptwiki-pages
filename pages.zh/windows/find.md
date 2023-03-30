# find 
## chatgpt 
find命令是一个用于在指定路径下查找文件和目录的命令，在Linux和Unix操作系统中广泛应用。通常用于查找特定名称、日期、所有者、权限等属性的文件，也可以使用正则表达式进行模式匹配搜索。

常用的find命令选项和参数包括：

- -name：按照文件名进行查找，支持shell通配符，例如find /path -name "*.txt"查找/path路径下所有以.txt后缀结尾的文件。
- -type：按照文件类型进行查找，支持f（普通文件）、d（目录）、l（符号链接）等选项。
- -mtime/-mmin：按照修改时间进行查找，-mtime后跟时间天数，-mmin后跟时间分钟数，例如find /path -mtime +7查找/path路径下7天前修改过的文件。
- -user/-group：按照所有者或所属组进行查找，-user后跟用户名，-group后跟组名。
- -perm/-atime/-ctime：按照权限、访问时间、创建时间进行查找，-perm后接数字表示具有该权限的文件，-atime/-ctime后接时间天数表示指定时间之前访问/创建的文件。

除了以上常见参数，find命令还支持多种操作符，例如：

- -and：逻辑与
- -or：逻辑或
- -not：逻辑非

例如find /path -name "*.txt" -o -name "*.log"查找/path路径下所有以.txt或.log结尾的文件。

另外，find命令还可以与-exec结合使用，执行指定的命令，例如find /path -name "*.txt" -exec ls -l {} \;在/path路径下查找所有以.txt结尾的文件并打印详细信息。{}表示匹配到的文件名，\;表示命令结束标识符。

总之，find命令是一个功能强大的文件查找工具，在操作系统维护、数据备份等场景中非常有用。 

## tldr 
 
> 在一个或多个文件里查找指定字符串。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/find>.

- 查找包含指定字符串的行：

`find {{字符串}} {{文件或目录的路径}}`

- 查找不包含指定字符串的行：

`find {{字符串}} {{文件或目录的路径}} /v`

- 显示包含指定字符串的行的总数：

`find {{字符串}} {{文件或目录的路径}} /c`

- 显示匹配的行的行数：

`find {{字符串}} {{文件或目录的路径}} /n`
