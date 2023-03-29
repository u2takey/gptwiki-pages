# mvn 
## chatgpt 
mvn是Maven命令行工具的缩写。Maven是开源的项目管理和构建工具，可以帮助您自动化构建、测试和部署Java应用程序。以下是一些常见的mvn命令和它们的作用：

- mvn clean：清除先前构建的所有文件和目录，使得可以从头开始重新构建
- mvn compile：编译源代码
- mvn test：运行测试
- mvn package：将编译的源代码打包成可执行的JAR文件或WAR文件
- mvn install：将打包后的JAR或WAR文件安装到本地Maven仓库，以便其他项目可以使用它
- mvn deploy：将JAR或WAR文件部署到Maven仓库的远程服务器，以供其他人使用

还有许多其他的mvn命令可以使用，例如mvn dependency:tree来查看项目中的依赖关系，mvn site可以为项目生成一个网站，列出其文档和其他相关信息等等。和其他命令行工具一样，您可以在终端中键入“mvn help”来获取关于mvn命令的详细信息。 

## tldr 
 
> Apache Maven.
> 用于构建和管理基于 Java 的项目的工具。
> 更多信息：<https://maven.apache.org>.

- 编译项目：

`mvn compile`

- 将编译后的代码打包成可分发格式，比如 `jar`：

`mvn package`

- 编译和打包，跳过单元测试：

`mvn package -DskipTests`

- 在本地 maven 存储库中安装构建的包（这也会调用 compile 和 package 命令）：

`mvn install`

- 从目标目录中删除构建工件，通常用来清理之前的编译结果：

`mvn clean`

- 执行清理操作，然后进行编译打包：

`mvn clean package`

- 执行清理操作并使用给定的构建配置打包代码，比如 `profileId` 如果有 dev、test、pro，可以指定其中一个 `profileId` 用来选择具体执行环境：

`mvn clean -P{{profileId}} package`

- 使用 main 方法运行一个类：

`mvn exec:java -Dexec.mainClass="{{com.example.Main}}" -Dexec.args="{{参数1 参数2}}"`
