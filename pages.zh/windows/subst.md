# subst 
## chatgpt 
命令 "subst" 用于将一个驱动器字母分配给指定路径，使得该路径可以被视为一种可识别的本地驱动器。这个命令也可以用来取消已分配的驱动器字母。

"subst" 的具体使用方式如下：

- 命令格式

subst [驱动器字母：] [路径]

- 参数说明

[驱动器字母：]：可选参数，指定要分配的驱动器字母，如果省略，则分配的是下一个可用的驱动器字母。

[路径]：必选参数，指定要分配驱动器字母的路径。

- 示例

1. 将 C:\Windows\System32\drivers 分配给驱动器字母 X：

subst X: C:\Windows\System32\drivers

执行该命令后，就可以通过 X: 来访问 C:\Windows\System32\drivers 目录下的文件。

2. 取消已分配的驱动器字母：

subst X: /D

执行该命令后，就会取消已分配给驱动器字母 X 的路径。 

## tldr 
 
> 将路径与虚拟驱动器号关联。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/subst>.

- 列出已激活的关联：

`subst`

- 添加一个关联：

`subst {{Z:}} {{C:\Python2.7}}`

- 删除一个关联：

`subst {{Z:}} /d`
