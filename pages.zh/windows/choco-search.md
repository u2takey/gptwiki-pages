# choco search 
## chatgpt 
choco search是Chocolatey软件包管理器中的一个命令，用于在Chocolatey的软件包库中搜索软件包。 

该命令的语法如下：

choco search <搜索条件> [<选项>]

其中，<搜索条件>可以是软件包名称或关键字，支持通配符匹配。

例如，要搜索名为Firefox的软件包，可以执行以下命令：

choco search firefox

搜索结果将包含所有与“firefox”有关的软件包。

该命令还支持几个选项，例如：

- -by=<属性>：按照指定的属性（例如，名称、版本等）排序搜索结果。
- -idonly：只返回软件包的ID而不是其完整的元数据。 

总之，choco search是一个非常实用的命令，可以帮助用户快速查找他们需要的软件包。 

## tldr 
 
> 使用 Chocolatey 搜索一个本地或远程的包。
> 更多信息：<https://chocolatey.org/docs/commands-search>.

- 搜索一个包：

`choco search {{查询语句}}`

- 搜索一个本地的包：

`choco search {{查询语句}} --local-only`

- 只显示包含完全匹配的结果：

`choco search {{查询语句}} --exact`

- 自动确认所有提示：

`choco search {{查询语句}} --yes`

- 从自定义的源处搜索包：

`choco search {{查询语句}} --source {{源 URL|别名}}`

- 提供一个用户名和密码来进行验证：

`choco search {{查询语句}} --user {{用户名}} --password {{密码}}`
