# jar 
## chatgpt 
jar是Java自带的打包工具，可以将多个Java类、资源文件和元数据打包成一个JAR文件。JAR文件是一种压缩文件格式，其中包含了Java代码、类文件、图像、音频等多种资源。JAR文件可以被Java虚拟机（JVM）加载和执行。

以下是使用jar命令的常见用法：

1. 创建JAR文件：使用“jar cvf”命令创建JAR文件，例如：jar cvf MyJar.jar MyFiles

    这将创建一个名为MyJar.jar的JAR文件，其中包含MyFiles目录下的所有文件。

2. 查看JAR文件内容：使用“jar tf”命令查看JAR文件内容，例如：jar tf MyJar.jar

    这将列出MyJar.jar中包含的所有文件和目录。

3. 解压缩JAR文件：使用“jar xvf”命令解压缩JAR文件，例如：jar xvf MyJar.jar

    这将解压缩MyJar.jar中的所有文件到当前目录下。

4. 添加文件到JAR文件：使用“jar uvf”命令添加文件到现有的JAR文件中，例如：jar uvf MyJar.jar MyNewFile.class

    这将将MyNewFile.class文件添加到名为MyJar.jar的JAR文件中。

5. 删除JAR文件中的文件：使用“jar d”命令在现有的JAR文件中删除文件，例如：jar d MyJar.jar MyOldFile.class

    这将从名为MyJar.jar的JAR文件中删除MyOldFile.class文件。

6. 运行JAR文件：在命令行中使用“java -jar”命令运行JAR文件，例如：java -jar MyJar.jar

    这将执行名为MyJar.jar的JAR文件中的主类。 

## tldr 
 
> Java 应用程序 / 类库打包程序。
> 更多信息：<https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

- 将当前目录中的所有文件递归归档到 `.jar` 文件中：

`jar cf {{file.jar}} *`

- 将 `.jar` / `.war` 文件解压缩到当前目录：

`jar -xvf {{file.jar}}`

- 列出 `.jar` / `.war` 文件内容：

`jar tf {{path/to/file.jar}}`

- 列出带有详细输出的 `.jar` / `.war` 文件内容：

`jar tvf {{path/to/file.jar}}`
