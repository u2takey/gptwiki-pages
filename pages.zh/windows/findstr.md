# findstr 
## chatgpt 
findstr 是一个 Windows 命令，用于在文本文件或标准输入中搜索指定字符串模式，并将包含匹配模式的行输出到标准输出。此命令常用于在大型文件夹或目录中查找指定的字符串，也可以用于筛选和处理文本数据。

findstr 命令有以下常用的选项和参数：

- /C：指定查找的字符串。可以使用多个 /C 选项来指定多个查找字符串。
- /I：不区分大小写搜索。
- /N：输出匹配行的行号。
- /V：不匹配选项。输出不包含指定字符串的行。
- /M：仅输出匹配字符串的文件名。
- /R：使用正则表达式匹配搜索。
- /S：递归搜索子目录。
- /X：精确匹配整个行，而不是仅查找出现在行中的字符串。

示例：
1. 查找包含字符串 "example" 的文件，并输出行号：

   findstr /N "example" c:\path\to\file.txt

2. 查找包含字符串 "hello" 的文件，并将匹配到的所有行输出到另一个文件：

   findstr "hello" *.txt > result.txt

3. 使用正则表达式匹配查找文件中以 "aaa" 和 "bbb" 开头的行：

   findstr /R "^aaa|^bbb" c:\path\to\file.txt

4. 递归搜索目录中所有文件，并查找包含字符串 "example" 的文件：

   findstr /S "example" c:\path\to\folder\*.*

5. 查找包含字符串 "hello" 和 "world" 的行，并将结果输出到另一个文件：

   findstr /C:"hello" /C:"world" input.txt > output.txt

注意：findstr 命令的选项和参数可以根据需要进行组合使用，以满足具体的搜索需求。 

## tldr 
 
> 在一个或多个文件中查找指定的文本。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/findstr>.

- 在所有文件中查找以空格分隔的字符串：

`findstr "{{查询语句 查询语句 ..}}" *`

- 以递归方式在所有文件中查找以空格分隔的字符串：

`findstr /s "{{查询语句 查询语句 ..}}" *`

- 查找时不区分大小写：

`findstr /i "{{查询语句}}" *"`

- 使用正则表达式搜索：

`findstr /r "{{正则表达式}}" *`

- 在所有文本文件中查找文字字符串（包含空格）：

`findstr /c:"{{查询语句}}" *.txt`

- 只查找完全匹配的行：

`findstr /x "{{查询语句}}" *`

- 显示匹配的行的行数：

`findstr /n "{{查询语句}}" *`

- 只显示匹配的文件名：

`findstr /m "{{查询语句}}" *`
