# mdutil 
## chatgpt 
mdutil是macOS系统中的一个命令行实用工具，用于管理和操作本地Spotlight搜索引擎的元数据存储。它有以下常用选项和参数：

常用选项：

- -i：显示Spotlight搜索引擎的信息，包括状态、自动激活和安装的卷。
- -s ：指定搜索卷的MDS状态，可以设置为on或off。
- -E：强制重新建立指定卷的元数据缓存。
- -d：禁用指定卷的Spotlight搜索引擎。
- -a：激活所有支持的Spotlight搜索引擎，包括用户配置的搜索卷和所有重新连接的搜索卷。

常用参数：

- volume：指定要管理的卷的路径。
- -n：仅列出要执行操作的项，而不实际执行它们。

示例：

1. 显示Spotlight搜索引擎的信息：

```
mdutil -i
```

2. 禁用指定卷的Spotlight搜索引擎：

```
mdutil -d /Volumes/Macintosh HD
```

3. 强制重新建立指定卷的元数据缓存：

```
mdutil -E /Volumes/Macintosh HD
```

注意：使用mdutil命令需要管理员权限。 

## tldr 
 
> 管理 Spotlight（聚焦搜索）用于搜索的索引数据。
> 更多信息：<https://ss64.com/osx/mdutil.html>.

- 显示指定卷（'/'）的索引状态：

`mdutil -s {{/}}`

- 打开 / 关闭给定卷的 Spotlight 索引：

`mdutil -i {{on|off}} {{指定卷文件夹}}`

- 清除索引数据并重新建立索引：

`mdutil -E {{指定卷文件夹}}`
