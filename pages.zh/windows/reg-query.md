# reg query 
## chatgpt 
命令：reg query

作用：查询注册表

使用说明：

1. 命令语法：reg query keyname [/v valuename] [/s]

2. keyname是指注册表中指定子项的路径。

3. /v参数可用于指定要查询的值的名称。

4. /s参数可用于在子目录中搜索指定的子项和值。

5. 如果未指定/v参数，则所有值将被列出。

6. 如果仅指定keyname，则子项将被列出。

7. 如果未指定keyname，则注册表中的根将被列出。

8. 命令输出包括子项和其值的名称、类型和数据。

示例：

1. 列出注册表中"HKEY_LOCAL_MACHINE\SOFTWARE"键下的所有子项

reg query HKEY_LOCAL_MACHINE\SOFTWARE

2. 列出注册表中"HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion"键下的所有值

reg query HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion

3. 列出注册表中"HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion"键下的"ProductName"值的数据

reg query HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion /v ProductName

4. 在"HKEY_LOCAL_MACHINE\SOFTWARE"键下递归搜索所有包含"Microsoft"的子项和值

reg query HKEY_LOCAL_MACHINE\SOFTWARE /s /f Microsoft 

## tldr 
 
> 显示注册表中键和子键的值。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-query>.

- 显示一个键中的所有值：

`reg query {{键名}}`

- 显示键中指定的值：

`reg query {{键名}} /v {{值}}`

- 显示指定键和其子键中的所有的值：

`reg query {{键名}} /s`

- 搜索与特定模式匹配的键和值：

`reg query {{键名}} /f "{{查询语句}}"`

- 显示与指定数据类型匹配的键的值：

`reg query {{键名}} /t {{类型}}`
