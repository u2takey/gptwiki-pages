# xattr 
## chatgpt 
xattr 命令是在 macOS 和 Linux 操作系统中用于管理扩展属性的命令。扩展属性是与文件或目录关联的键值对，可以存储任何类型的数据，例如文件作者、编辑日期、拍摄地点等等。

下面是一些常见的 xattr 命令选项和用途：

- -l：列出所有扩展属性的名称和值。
- -w：设置或修改扩展属性的值。
- -r：递归地处理目录中的所有文件和子目录。
- -d：删除指定的扩展属性。
- -c：清空所有扩展属性。

一些示例：

1. 显示文件的所有扩展属性，使用命令：

```
xattr -l filename
```

2. 设置文件的某个扩展属性，使用命令：

```
xattr -w attr_name "value" filename
```

3. 删除文件中的一个扩展属性，使用命令：

```
xattr -d attr_name filename
```

4. 清空文件的所有扩展属性，使用命令：

```
xattr -c filename
```

需要注意的是，某些扩展属性是系统自动生成的，例如 com.apple.quarantine，用于标记从互联网下载的文件，以提醒用户谨慎打开这些文件。修改或删除这些系统自动生成的属性可能导致不可预测的影响。因此，在操作扩展属性时，应格外小心，确保不会影响系统的正常运行和文件的完整性。 

## tldr 
 
> 用于扩展文件系统属性的实用程序。
> 更多信息：<https://ss64.com/osx/xattr.html>.

- 列出 键：值 列表，显示指定文件的值扩展属性：

`xattr -l {{文件名}}`

- 为给定文件写入属性：

`xattr -w {{属性键名}} {{属性值}} {{文件名}}`

- 从给定文件中删除属性：

`xattr -d {{com.apple.quarantine}} {{文件名}}`

- 从给定文件中删除所有扩展属性：

`xattr -c {{文件名}}`

- 递归删除给定目录中文件的属性：

`xattr -rd {{属性键名}} {{目录}}`