# make 
## chatgpt 
make是一种流行的构建工具，这个命令会按照Makefile文件中的规则来构建指定的目标。

在Makefile中，每个目标都定义了其所需的依赖关系和构建规则。Make工具会自动跟踪这些依赖关系并仅更新需要更新的内容。这使得Make非常适合管理大型项目和复杂的构建流程。

make命令通常使用以下语法：

```
make [options] [target]
```

其中，options是可选参数，target是要构建的目标。如果未指定目标，则构建默认目标。一些通用的Make选项包括：

- -f：指定Makefile文件的名称或路径。
- -n：仅列出将要执行的命令，而不实际执行它们。
- -s：静默模式，只输出关键信息。

在运行make命令时，它会读取Makefile文件并执行定义的规则以构建指定目标。这些规则可能包括编译和链接代码，复制或移动文件，或执行任何其他必要的操作。通常，Make会跟踪每个目标及其依赖项的时间戳，以确保仅在需要时才更新文件。

一些常见的make目标包括：

- all：构建项目中的所有目标。
- clean：删除所有生成的文件和目标。
- install：将项目安装在系统上。
- test：运行项目的测试套件。

通过灵活的规则和选项，make可以轻松地管理大型项目中的构建，提高项目的可靠性和可维护性。 

## tldr 
 
> Makefile 文件描述目标的任务运行器。
> 通常用于控制源代码中可执行文件的编译。
> 更多信息：<https://www.gnu.org/software/make/manual/make.html>.

- 调用 Makefile 中指定的第一个目标（通常命名为 "all"）：

`make`

- 调用指定目标：

`make {{目标}}`

- 调用一个指定的目标，一次并行执行 4 个作业：

`make -j{{4}} {{目标}}`

- 使用指定的 Makefile 文件：

`make --file {{文件}}`

- 从另一个目录执行 make ：

`make --directory {{文件夹}}`

- 即使源文件未更改，也强制执行目标：

`make --always-make {{目标}}`

- 覆盖在 Makefile 中定义的环境变量：

`make --environment-overrides {{目标}}`
