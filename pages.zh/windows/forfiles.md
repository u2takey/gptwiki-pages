# forfiles 
## chatgpt 
forfiles命令是一种用于在文件夹中搜索文件并对其进行操作的命令。以下是forfiles命令的一些常见用法：

1. 批量删除文件：

    forfiles /p "folder_path" /s /m *.* /c "cmd /c del @path"

    此命令将递归搜索文件夹的每个子文件夹，使用del命令删除所有文件。

2. 批量复制文件：

    forfiles /p "folder_path" /s /m *.txt /c "cmd /c copy @path new_folder_path"

    此命令将递归搜索文件夹的每个子文件夹，使用copy命令将所有txt文件复制到指定的新文件夹中。

3. 批量修改文件名：

    forfiles /p "folder_path" /s /m *.txt /c "cmd /c rename @file new_file_name.txt"

    此命令将递归搜索文件夹的每个子文件夹，使用rename命令将所有txt文件的名称修改为指定的名称。

4. 批量压缩文件：

    forfiles /p "folder_path" /s /m *.txt /c "cmd /c 7za a -tzip archive.zip @path"

    此命令将递归搜索文件夹的每个子文件夹，使用7-Zip压缩软件将所有txt文件压缩成一个zip归档文件。

总之，forfiles命令是一种快速、灵活的文件管理工具，可用于执行各种操作，如删除、复制、重命名、压缩等。 

## tldr 
 
> 选择一个或多个文件以执行指定的命令。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/forfiles>.

- 在当前的目录中寻找文件：

`forfiles`

- 在一个指定目录中寻找文件：

`forfiles /p {{目录的路径}}`

- 为每个文件执行指定的命令：

`forfiles /c "{{命令}}"`

- 使用通配符来寻找指定的文件：

`forfiles /m {{通配符}}`

- 递归寻找文件：

`forfiles /s`

- 搜索超过 5 天的文件：

`forfiles /d {{+5}}`
