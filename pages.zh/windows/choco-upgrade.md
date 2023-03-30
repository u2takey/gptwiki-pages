# choco upgrade 
## chatgpt 
choco upgrade命令是Chocolatey包管理器的一种命令，用于升级已经安装的软件包。该命令用于更新已经安装的软件包到最新版本。它会检查可用的更新并下载最新版本，然后安装新版本。

要运行choco upgrade命令，可以使用以下语法：

```
choco upgrade <package name>
```

其中，<package name>是您要升级的软件包的名称。如果要升级所有已安装的软件包，则可以运行以下命令：

```
choco upgrade all
```

该命令将升级所有已安装的软件包。

重要提示：在升级软件包之前，请确保您已创建备份，以防升级过程中出现问题导致数据丢失或软件不可用。 

## tldr 
 
> 使用 Chocolatey 升级一个或多个包。
> 更多信息：<https://chocolatey.org/docs/commands-upgrade>.

- 升级一个或多个用空格分隔的软件包：

`choco upgrade {{包名 包名 ..}}`

- 将一个包升级到指定版本：

`choco upgrade {{包名}} --version {{版本号}}`

- 升级全部包：

`choco upgrade all`

- 升级除指定的用逗号分隔的包之外的所有包：

`choco upgrade all --except "{{包名 , 包名 ..}}"`

- 自动确认所有提示：

`choco upgrade {{包名}} --yes`

- 从自定义源处升级包：

`choco upgrade {{包名}} --source {{源 URL|别名}}`

- 提供一个用户名和密码来进行验证：

`choco upgrade {{包}} --user {{用户名}} --password {{密码}}`
