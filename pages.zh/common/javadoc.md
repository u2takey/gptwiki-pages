# javadoc 
## chatgpt 
javadoc是Java SDK自带的文档生成工具。它可以根据Java源代码自动生成API文档，可以从文档中了解Java类、接口、方法、字段的详细信息。javadoc可以生成HTML、PDF、CHM等各种格式的API文档，使用简单方便，大大提高了Java开发的效率。

javadoc命令的用法如下：

```
javadoc [options] [packagenames] [sourcefiles] [@files]
```

其中，`[options]`是选项参数，包括了许多常用的选项，如-javadocExecutable、-docencoding、-encoding、-charset、-locale、-link、-linkoffline、-private等等，可以根据需要进行配置。

`[packagenames]`是需要生成API文档的包名，多个包名之间用空格分隔。

`[sourcefiles]`是需要生成API文档的Java源码文件，多个文件之间用空格分隔。

`[@files]`是指定包含命令行选项的文件，一行一个选项。

下面是一些常用的javadoc命令选项：

- `-d`：指定输出目录。
- `-sourcepath`：指定源文件路径。
- `-subpackages`：指定需要生成API文档的子包。
- `-classpath`：指定编译后的类文件路径。
- `-exclude`：指定不需要生成API文档的类名。
- `-overview`：指定概述文件的路径。
- `-windowtitle`：指定文档窗口标题。
- `-doctitle`：指定文档标题。
- `-header`：指定页眉。
- `-footer`：指定页脚。
- `-bottom`：指定文档底部。
- `-author`：生成文档时包含作者信息。
- `-version`：生成文档时包含版本信息。
- `-private`：生成文档时包含私有成员。

使用javadoc命令生成API文档有以下步骤：

1. 编写Java源代码。
2. 在源代码中添加注释（注释格式必须符合Javadoc规范）。
3. 执行javadoc命令，生成API文档。
4. 打开文档，查看Java类、接口、方法、字段等详细信息。

总之，javadoc是非常重要的Java开发工具之一，可以帮助开发者更好地了解和使用Java标准库，提高开发效率和代码可读性。 

## tldr 
 
> 从源代码以 HTML 格式生成 Java API 文档。
> 更多信息：<https://docs.oracle.com/en/java/javase/19/docs/specs/man/javadoc.html>.

- 生成 Java 源代码的文档并将结果保存在文件夹中：

`javadoc -d {{path/to/directory/}} {{path/to/java_source_code}}`

- 生成指定编码的文档：

`javadoc -docencoding {{UTF-8}} {{path/to/java_source_code}}`

- 生成文档时，排除掉某些软件包：

`javadoc -exclude {{package_list}} {{path/to/java_source_code}}`
