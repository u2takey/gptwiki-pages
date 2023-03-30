# choco list 
## chatgpt 
choco list是Chocolatey软件包管理器的命令之一，它列出了已安装或可安装的软件包。更具体地说，它列出了位于Chocolatey库中的所有软件包，无论它们是否已经被安装在本地计算机上。 

该命令的语法为： 

```
choco list [<pkgFilter>] [<options/switches>]
```

其中， \<pkgFilter\> 是可选的，用于指定要列出的特定软件包或软件包模式，例如： 

- “python”：只列出名字包含“python”的软件包
- “googlechrome 42.0”：只列出版本号为“42.0”的Google Chrome浏览器
- “python*,visualstudiocode”：列出所有名字包含“python”的软件包以及“Visual Studio Code”
- “all ”：列出所有可用的软件包

\<options/switches\> 也是可选的，用于指定其他可用的选项和开关，例如： 

- “—local-only”：只列出已经在本地计算机上安装的软件包
- “—exact”：只列出名称完全匹配\<pkgFilter\>的软件包
- “—idonly”：只显示软件包ID
- “—include-programs=”：只列出已安装的指定程序的相关软件包

总之，choco list命令是在Chocolatey库中列出软件包的一种方便而实用的方式，它可以快速地帮助您找到需要的软件包并进行安装或升级。 

## tldr 
 
> 使用 Chocolatey 显示包列表。
> 更多信息：<https://chocolatey.org/docs/commands-list>.

- 列出所有可用的包：

`choco list`

- 列出所有本地已安装的包：

`choco list --local-only`

- 显示包含本地程序的列表：

`choco list --include-programs`

- 只显示已批准的包：

`choco list --approved-only`

- Specify a custom source to display packages from 指定一个源来显示包列表：

`choco list --source {{源 URL|别名}}`

- 提供一个用户名和密码来进行验证：

`choco list --user {{用户名}} --password {{密码}}`
