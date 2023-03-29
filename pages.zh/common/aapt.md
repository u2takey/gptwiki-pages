# aapt 
## chatgpt 
aapt是Android Asset Packaging Tool的缩写，是一个用于Android应用程序打包的命令行工具。

aapt主要用于将应用程序资源打包成一个APK文件，同时可以解析APK文件中的信息，并根据需要添加、删除或修改APK文件中的资源。具体来说，aapt可以执行以下操作：

1. 编译应用程序资源：将Android应用程序中的所有资源（如布局、字符串、图片、Manifest文件等）编译成二进制文件，供应用程序在运行时使用。

2. 打包资源：将所有编译后的资源打包成一个APK文件，并将APK文件签名以保证数据的完整性和安全性。

3. 解析APK文件：从APK文件中提取出应用程序的Manifest文件，资源文件、代码等信息，便于分析和修改应用程序。

4. 修改APK文件：可以使用aapt给APK文件中添加、删除或修改资源文件，以及修改Manifest文件中的信息。

5. 验证APK文件：可以使用aapt来验证APK文件是否符合Android系统的规范和要求，并检查是否存在安全漏洞。

总之，aapt是一个非常重要的工具，它将应用程序打包成APK文件，使得应用程序可以在Android系统上运行，并且也方便了开发人员进行资源的编译、打包和管理。 

## tldr 
 
> 安卓资源包工具（Android Asset Packaging Tools）。
> 该工具可以查看，创建，更新资源压缩包（zip, jar, apk）。
> 更多信息：<https://elinux.org/Android_aapt>.

- 列出资源压缩包里的内容：

`aapt list {{路径/到/应用.apk}}`

- 查看 APK 包内指定的内容（版本，权限许可等）：

`aapt dump badging {{路径/到/应用.apk}}`

- 打包生成资源压缩包：

`aapt package -F {{路径/到/应用.apk}} {{路径/到/目录}}`
