# lvs 
## chatgpt 
lvs命令是Linux中用于显示逻辑卷信息的命令，lvs是Logical Volume Scan的缩写。它主要用于列出指定卷组的逻辑卷信息，包括逻辑卷名称、逻辑卷大小、它们使用的物理卷以及它们的状态和剩余空间等等。

具体选项说明：

- -a或--all：列出所有逻辑卷。
- -o或--options：以指定的格式显示所需的列名。
- -O或--sort：按指定的逗号分隔符分隔的字段排序结果。
- -S或--separator：指定不同单元格之间的分隔符。
- -v或--verbose：提供详细的输出信息，包括设备信息、UUID等等。

示例：

1. 列出所有逻辑卷的信息：

```
lvs
```

2. 列出逻辑卷的名称和大小

```
lvs -o lv_name,lv_size
```

3. 按剩余空间列出逻辑卷

```
lvs --sort lv_free
```

4. 提供详细的输出信息

```
lvs -v
``` 

## tldr 
 
> 显示逻辑卷信息。
> 另见：`lvm`.
> 更多信息：<https://man7.org/linux/man-pages/man8/lvs.8.html>.

- 显示逻辑卷信息：

`lvs`

- 显示所有逻辑卷：

`lvs -a`

- 改变默认显示以显示更多细节：

`lvs -v`

- 只显示特定字段：

`lvs -o {{域名 1}},{{域名 2}}`

- 将字段附加到显示：

`lvs -o +{{域名}}`

- 抑制标题行：

`lvs --noheadings`

- 使用特殊分隔符分隔特定字段：

`lvs --separator {{=}}`
