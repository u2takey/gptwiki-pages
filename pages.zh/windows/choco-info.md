# choco info 
## chatgpt 
choco info是Chocolatey包管理器的命令之一，用于显示有关特定软件包的详细信息。该命令可帮助您查找软件包的名称，版本号，作者，包含文件，依赖项和其他有关其功能的详细信息。

具体来说，使用choco info命令，您可以：

1. 查找软件包的名称和版本号
2. 查看软件包的作者和许可证信息
3. 确定是否有可用的新版本更新
4. 查看软件包的依赖项和建议项
5. 确定软件包是否已安装并在哪个路径上安装

例如，如果要获取有关“notepadplusplus”软件包的信息，则可以在命令行中输入以下内容：

choco info notepadplusplus

该命令将返回软件包的详细信息，例如名称，版本号，作者和许可证信息，文件和文件夹结构和依赖项列表。 

## tldr 
 
> 显示有关 Chocolatey 包的详细信息。
> 更多信息：<https://chocolatey.org/docs/commands-info>.

- 显示指定包的信息：

`choco info {{包名}}`

- 显示一个本地已安装包的信息：

`choco info {{包名}} --local-only`

- 从一个自定义的源来获取包的信息：

`choco info {{包名}} --source {{源 URL|别名}}`

- 提供一个用户名和密码来进行验证：

`choco info {{包名}} --user {{用户名}} --password {{密码}}`
