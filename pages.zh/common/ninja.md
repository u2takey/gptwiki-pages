# ninja 
## chatgpt 
ninja 是一个快速、轻量级的构建工具。与传统的构建工具（如 GNU make）不同，ninja 不需要解析整个 Makefile 文件，构建速度更快。

ninja 的语法与 Makefile 类似，但更加简洁和易于理解。使用 ninja 构建项目的流程如下：

1. 编写一个名为 build.ninja 的文件，描述要构建的所有目标文件，以及它们之间的依赖关系和构建规则。

2. 运行命令 `ninja` 或 `ninja <target>`，ninja 将根据 build.ninja 中的描述自动构建所有目标文件。

3. 如果您修改了某些源文件，并且需要重新构建某些目标文件，您可以运行 `ninja <target>` 重新构建指定的目标文件。

ninja 可以自动检测源文件和依赖文件的变化，并只重新构建必要的目标文件，从而节省时间和资源。此外，ninja 还可以并行构建多个目标文件，提高构建效率。 

## tldr 
 
> 一个快速的构建系统。
> 更多信息：<https://ninja-build.org/manual.html>.

- 在当前目录下构建：

`ninja`

- 在指定的目录中构建一个程序：

`ninja -C {{路径}}`

- 查看 target（如 `install` 和 `uninstall`）：

`ninja -t targets`

- 查看帮助：

`ninja -h`
