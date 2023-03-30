# glibtool 
## chatgpt 
glibtool 是一个用于构建共享库（shared library）的工具，它是 GNU libtool 的一部分。它通过管理共享库之间的依赖关系，使得构建共享库更容易。 glibtool 可以为多个平台上的不同编译器生成共享库。

glibtool 可以使用以下选项：

- `-c`：仅编译不链接。
- `-dlopen`：生成动态链接库时使用 dlopen() 系统调用打开库，代替默认的 lt_dlopen() 函数。
- `-export-symbols`：指定应该被导出的符号列表，这些符号可以被其他程序链接使用。
- `-install_name`：指定库的安装路径。
- `-L`：指定库目录的位置。
- `-dynamic`：生成动态链接库，而不是静态库。
- `-static`：生成静态库。

除此之外，glibtool 还可以使用一些其他的选项，用于控制编译生成共享库的行为。 

## tldr 
 
> 这是 `-p linux libtool` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux libtool`
