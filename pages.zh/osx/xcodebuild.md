# xcodebuild 
## chatgpt 
xcodebuild是Xcode的一部分，是一个用于构建、分析、测试和打包iOS、macOS、watchOS和tvOS应用程序的命令行工具。它可以让开发者在终端中运行大多数Xcode功能，而不必依赖于Xcode的图形用户界面。

xcodebuild可以支持以下功能：

1.构建：编译和构建Xcode项目或工作区。可以通过指定目标，配置和构建选项来构建应用程序。

2.测试：运行Xcode项目或工作区中的单元测试、UI测试和性能测试。可以通过指定测试过滤器和Xcode模拟器来测试应用程序。

3.打包：将iOS、macOS、watchOS和tvOS应用程序打包成.ipa或.app文件。可以使用xcodebuild来打包应用程序并将其上传到App Store。

4.分析：在构建应用程序时，xcodebuild可以生成分析报告，帮助开发者找到应用程序中的性能问题和内存泄漏。

xcodebuild支持大量的参数和选项来定制构建、测试和打包过程。它通常与CI/CD流程一起使用，以便自动化地构建、测试和部署应用程序。 

## tldr 
 
> 构建 Xcode 项目。
> 更多信息：<https://developer.apple.com/library/archive/technotes/tn2339/_index.html>.

- 构建工作区：

`xcodebuild -workspace {{工作区名.工作区}} -scheme {{主题名}} -configuration {{配置名}} clean build SYMROOT={{SYMROOT_路径}}`

- 构建项目：

`xcodebuild -target {{目标名}} -configuration {{配置名}} clean build SYMROOT={{SYMROOT_路径}}`

- 显示 SDK：

`xcodebuild -showsdks`
