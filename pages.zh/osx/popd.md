# popd 
## chatgpt 
popd 命令用于从目录堆栈中删除并切换到上一个目录，详情如下：

1. 命令格式：popd

2. 作用：从目录堆栈中删除最近添加的目录并切换到上一个目录

3. 注意事项：

- 如果没有在任何目录中建立目录堆栈，则会显示错误消息。
- 如果只有一个目录在目录堆栈中，那么执行 popd 命令后目录堆栈将为空。
- popd 是一个 shell 内置命令，可以在任何 shell 中使用。

4. 常用选项：

- -n：不切换目录，只是从目录堆栈中删除最近添加的目录。

5. 示例：

- 示例1：在命令行中使用 popd 命令删除并切换到上一个目录。

```shell
$ cd /path/to/dir1
$ cd /path/to/dir2
$ popd       # 切换到 /path/to/dir1 目录，并从目录堆栈中删除 /path/to/dir2
```

- 示例2：在命令行中使用 popd -n 命令仅从目录堆栈中删除最近添加的目录，但不切换目录。

```shell
$ cd /path/to/dir1
$ cd /path/to/dir2
$ popd -n    # 目录堆栈只剩 /path/to/dir1，不切换目录
``` 

## tldr 
 
> 通过 pushd shell 内置程序删除目录堆栈中的目录。

- 从堆栈中删除顶部目录，并用 `cd` 跳转到该目录：

`popd`

- 删除第 n 个目录（从零开始，以用 `dirs` 打印的列表左侧开始）：

`popd +N`

- 删除第 n 个目录（从零开始，以用 `dirs` 打印的列表右侧开始）：

`popd -N`