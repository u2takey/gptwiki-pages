# scoop bucket 
## chatgpt 
scoop bucket是scoop软件包管理器的命令之一，它用于管理scoop存储库中的存储桶(bucket)。

scoop存储库是一组称为“存储桶(bucket)”的Git存储库的集合，这些存储桶包含scoop软件包的定义文件。可以通过将新存储桶添加到scoop存储库来添加新的软件包，或通过更新现有存储桶中的软件包来修复错误或增加功能。

scoop bucket命令提供了以下子命令：

1. scoop bucket add [bucket-name] [bucket-url]: 将新存储桶添加到scoop存储库中，其中[bucket-name]为存储桶的名称，[bucket-url]为存储桶的Git仓库地址。

2. scoop bucket rm [bucket-name]: 从scoop存储库中删除指定的存储桶，其中[bucket-name]为存储桶的名称。

3. scoop bucket list: 列出scoop存储库中所有可用存储桶的名称。

4. scoop bucket known: 列出已知的所有scoop存储库，这些存储库包含scoop软件包的定义文件。

scoop bucket命令允许scoop用户管理他们安装的软件包，并且是一种非常有效的方法来安装、更新或删除软件包。 

## tldr 
 
> 管理 bucket: 包含描述 scoop 应如何安装应用程序的文件的 Git 存储库。
> 如果 Scoop 不知道 bucket 在哪里，则必须指定其存储库位置。
> 更多信息：<https://github.com/lukesampson/scoop/wiki/Buckets>.

- 列出所有正在使用的 bucket：

`scoop bucket list`

- 列出所有已知 bucket：

`scoop bucket known`

- 按名称添加一个已知 bucket：

`scoop bucket add {{名称}}`

- 通过名称和 Git 存储库 URL 添加未知 bucket：

`scoop bucket add {{名称}} {{https://example.com/repository.git}}`

- 按名称删除 bucket：

`scoop bucket rm {{名称}}`
