# reg delete 
## chatgpt 
命令：`reg delete`

该命令用于从Windows注册表中删除指定的键或值。

语法：

```
reg delete [<参数>] <键名> [/v <值名>] [/f]
```

参数：

- `<键名>`：要删除的键的完整路径。
- `/v <值名>`：要删除的值的名称。如果省略，则将删除整个键。
- `/f`：强制执行，无需进行确认。

示例：

1. 删除键：

```
reg delete HKEY_LOCAL_MACHINE\Software\Example
```

以上命令将删除注册表中 `HKEY_LOCAL_MACHINE\Software\Example` 键和其所有子键和值。

2. 删除值：

```
reg delete HKEY_CURRENT_USER\Software\Example /v MyValue
```

以上命令将删除 `HKEY_CURRENT_USER\Software\Example` 键下名为 `MyValue` 的值。

3. 强制删除：

```
reg delete HKEY_LOCAL_MACHINE\Software\Example /f
```

以上命令将强制删除 `HKEY_LOCAL_MACHINE\Software\Example` 键及其所有子键和值，无需进行确认。注意，此命令非常危险，需要谨慎操作。 

## tldr 
 
> 从注册表中删除键和值。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-delete>.

- 删除一个指定的键：

`reg delete {{键名}}`

- 删除键中指定的值：

`reg delete {{键名}} /v {{值}}`

- 递归删除指定键下所有的值：

`reg delete {{键名}} /va`

- 在没有提示的情况下递归删除键中所有的值：

`reg delete {{键名}} /f /va`
