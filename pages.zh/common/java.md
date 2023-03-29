# java 
## chatgpt 
java命令是Java开发工具包（JDK）提供的一个命令行工具，它用于执行Java应用程序或Java类。当用户编写Java程序并将其编译成字节码文件（.class文件）时，可以使用java命令来运行这些程序。

该命令的语法为：

java [options] classname [arguments]

其中，options表示可选参数，classname是要运行的Java类名，arguments是传递给类main()方法的参数。

java命令支持许多选项，其中一些常用的选项如下：

-cp或-classpath：指定Java程序运行时使用的路径或JAR包列表。
-Xmx或-maximum-memory：指定Java虚拟机（JVM）可用的最大内存。
-D<name>=<value>：定义系统属性名和值的方式。
-version：显示Java版本信息。
-help：显示命令帮助信息。

例如，要在设置了classpath的情况下运行MyClass.java类，可以使用以下命令：

java -classpath /path/to/my/class MyClass

这将会执行MyClass类的main()方法。

总之，java命令是Java开发中一个基本而且非常实用的命令，它允许用户在命令行界面执行Java程序。 

## tldr 
 
> Java 程序启动器。
> 更多信息：<https://docs.oracle.com/en/java/javase/19/docs/specs/man/java.html>.

- 通过提供类名称运行一个含有 main 函数的 java .class 程序：

`java {{类名称}}`

- 运行一个 .jar 程序：

`java -jar {{文件名.jar}}`

- 运行一个 .jar 程序并且在端口 5005 等待调试器：

`java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{文件名.jar}}`

- 显示 JDK, JRE 和 HotSpot 的版本：

`java -version`

- 显示详细的帮助：

`java -help`
