# choco new 
## chatgpt 
choco new是Chocolatey（一个Windows软件包管理器）中的一个命令，用于创建一个新的软件包规范。具体解释如下：

1.新建软件包规范

使用choco new命令，您可以创建一个新的软件包规范。这个规范描述了一个可安装软件的所有信息，包括软件名称、版本、安装程序、依赖项等。

2.便于构建软件包

创建软件包规范非常有用，因为它可以帮助您构建软件包。您可以使用这个规范作为一个模板，从而为每个软件包的构建提供相同的基础架构。

3.命令格式

使用choco new命令，您需要提供软件包名称作为参数。例如，若您要创建一个名为“example”的软件包规范，则命令应该如下所示：

choco new example

4.自动生成文件

使用该命令会自动为您创建一个新的目录，该目录包含一个nuspec文件和一个powershell脚本，其中包含软件包规范的基本信息和命令。

总之，choco new命令是用于创建一个新的软件包规范的Chocolatey命令，可以为您的软件包构建提供基础架构。 

## tldr 
 
> 使用 Chocolatey 生成新的包规范文件。
> 更多信息：<https://chocolatey.org/docs/commands-new>.

- 创建一个新的包框架：

`choco new {{包名}}`

- 创建一个新的指定版本的包：

`choco new {{包名}} --version {{版本号}}`

- 创建一个新的包并指定维护者的名字：

`choco new {{包名}} --maintainer {{维护者名字}}`

- 在指定目录下创建新的包：

`choco new {{包名}} --output-directory {{指定的目录路径}}`

- 创建一个新的包并指定其 32 位版和 64 位版的安装 URL：

`choco new {{package_name}} url="{{url}}" url64="{{url}}"`
