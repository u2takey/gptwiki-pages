# javac 
## chatgpt 
javac是Java编译器的命令，用于将Java源代码文件(.java)编译成Java字节码文件(.class)。具体使用方法如下：

1. 打开命令提示符或终端；

2. 使用cd命令切换到.java源文件所在的目录；

3. 输入javac命令，后跟需要编译的Java源代码文件名，例如：javac HelloWorld.java；

4. 如果编译成功，生成的字节码文件(.class)将会保存在同一目录下。

需要注意的是，如果源文件中引用了其他类或包，需要在同一目录下或classpath中包含这些类或包的源代码或字节码文件。另外，如果Java源文件和字节码文件的文件名不一致，需要在javac命令中显式指定文件名。 

## tldr 
 
> Java 程序编译器。
> 更多信息：<https://docs.oracle.com/en/java/javase/19/docs/specs/man/javac.html>.

- 编译一个 `.java` 文件：

`javac {{文件名.java}}`

- 编译多个 `.java` 文件：

`javac {{文件名1.java}} {{文件名2.java}} {{文件名3.java}}`

- 编译当前目录内所有 `.java` 文件：

`javac {{*.java}}`

- 编译一个 `.java` 文件并将生成的 class 字节码文件放入一个指定目录：

`javac -d {{路径/到/目录}} {{文件名.java}}`
