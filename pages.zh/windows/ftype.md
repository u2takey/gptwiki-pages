# ftype 
## chatgpt 
ftype命令用于显示或修改文件类型关联。在Windows中，每个文件都与一种特定的文件类型关联，这将决定在打开文件时应使用哪个应用程序。ftype命令显示每个文件类型的名称（称为文件类型名称）和相关应用程序的路径，以及该文件类型的其他属性。

ftype命令有两个主要的使用方式：

1. 显示所有文件类型关联：

要查看所有文件类型关联，请在命令提示符下输入以下命令：

```
ftype
```

该命令将在屏幕上列出所有已定义的文件类型名称与关联的应用程序。

2. 修改文件类型关联：

要更改某个文件类型的关联，请使用以下命令：

```
ftype [文件类型]=[应用程序路径及文件名]
```

例如，要将所有.ppt文件的默认应用程序更改为Microsoft PowerPoint，可以使用以下命令：

```
ftype pptfile="C:\Program Files\Microsoft Office\Office16\POWERPNT.EXE" "%1"
```

此命令将把.ppt文件的文件类型名称设置为pptfile，并将其关联到 C:\Program Files\Microsoft Office\Office16\POWERPNT.EXE 应用程序的路径中。

另一个常见的使用场景是将Windows默认浏览器更改为其他浏览器。例如，要将Chrome设置为默认浏览器，请使用以下命令：

```
ftype http="C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" -- "%1"
``` 

## tldr 
 
> 显示或修改用于文件扩展名关联的文件类型。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/ftype>.

- 显示所有文件类型的列表：

`ftype`

- 显示特定文件类型的关联程序：

`ftype {{文件类型}}`

- 设置特定文件类型的关联程序：

`ftype {{文件类型}}="{{可执行命令的路径}}"`
