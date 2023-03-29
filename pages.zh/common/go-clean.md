# go clean 
## chatgpt 
go clean是一个go命令，它用于从本地源码仓库中删除构建生成的对象文件和可执行文件。该命令的具体用法如下：

```
go clean [-i] [-r] [-n] [-x] [build flags] [packages]
```

其中，常用标志包括：

- -i：删除安装的包及其依赖的包。
- -r：递归删除所有依赖的包。
- -n：仅打印要执行的操作，而不实际执行。
- -x：打印执行的详细命令。
- build flags：与构建相关的标志。
- packages：需要执行清理操作的包的列表。

在执行go clean命令时，会清理生成的二进制文件、临时文件、缓存文件和测试生成的文件等。如果使用了-i标志，还会删除已经安装的包及其依赖的包。

总之，go clean命令可以帮助用户在代码构建过程中清理缓存和无用的文件，保证环境的整洁。 

## tldr 
 
> 移除目标文件和缓存文件。
> 更多信息：<https://golang.org/cmd/go/#hdr-Remove_object_files_and_cached_files>.

- 只打印移除命令，而不会真正移除任何东西：

`go clean -n`

- 删除编译缓存：

`go clean -cache`

- 删除所有测试结果缓存：

`go clean -testcache`

- 删除模块缓存：

`go clean -modcache`
