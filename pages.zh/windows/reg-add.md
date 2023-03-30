# reg add 
## chatgpt 
reg add是Windows中的一个命令，是用于添加或修改注册表项的命令。它可以用于创建新的注册表项、子项和值，以及修改现有的注册表项、子项和值。

该命令有以下语法格式：

```
REG ADD KeyName [/v ValueName | /ve] [/t DataType] [/d Data] [/f]
```

其中：

- KeyName：要添加或修改的注册表项的完整路径。例如，“HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run”。
- /v ValueName：要添加或修改的注册表值的名称。如果没有指定此参数，则默认为“default”。
- /ve：表示要对默认值进行修改。如果指定了此参数，则无需指定ValueName。
- /t DataType：要添加或修改的注册表值的数据类型。数据类型可以是REG_SZ（字符串）、REG_DWORD（双字）、REG_MULTI_SZ（多字符串）等。
- /d Data：要添加或修改的注册表值的数据。如果未指定此参数，则默认为null。
- /f：表示强制覆盖现有值或注册表项而不提示用户。

例如，以下是添加一个新值的示例：

```
REG ADD HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run /v MyProgram /t REG_SZ /d "C:\Program Files\MyProgram.exe"
```

这将在“HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run”位置创建一个名为“MyProgram”的新注册表值，其数据为“C:\Program Files\MyProgram.exe”。 

## tldr 
 
> 将新的键值添加到注册表中。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-add>.

- 添加一个新的注册表键：

`reg add {{键名}}`

- 在指定的键下添加新值：

`reg add {{键名}} /v {{值}}`

- Add a new value with specific data：

`reg add {{键名}} /d {{数据}}`

- 向具有特定数据类型的键添加新值：

`reg add {{键名}} /t {{类型}}`

- 在没有提示的情况下强制覆盖现有的注册表值：

`reg add {{键名}} /f`
