# apktool 
## chatgpt 
apktool是一个开源工具，用于反编译和重新打包Android应用程序，它可以将一个已经打包好的apk文件进行反编译，获取其中的资源文件、Java代码等，并允许您在将应用程序重新编译并打包成修改后的格式的同时进行修改，这在测试和开发期间非常有用。

apktool命令的基本用法如下：

1. 打开终端并导航到要解包的APK目录。

2. 运行以下命令：apktool d yourapk.apk。此命令将APK中的源代码和资源解包到指定的目录中。

3. 修改应用程序的源代码和资源。

4. 运行以下命令来重新打包已修改的文件：apktool b yourapk。

5. 然后重新签名您的应用程序。这通常需要使用其他工具，例如Jarsigner或Android Studio的构建选项。

需要注意的是，使用apktool可能会遇到一些问题，如不支持某些Android应用程序的版本，某些特殊的应用程序文件等，因此在使用它之前，最好阅读它的文档以获得更多信息。 

## tldr 
 
> APK 文件反编译工具。
> 更多信息：<https://ibotpeaches.github.io/Apktool/>.

- 反编译：

`apktool d {{应用.apk}}`

- 将一个文件夹打包为 apk 文件：

`apktool b {{路径/到/目录}}`

- 安装并存储框架：

`apktool if {{框架.apk}}`
