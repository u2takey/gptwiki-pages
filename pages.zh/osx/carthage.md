# carthage 
## chatgpt 
Carthage是一个iOS的依赖管理器，它允许你用Swift构建你的项目。 它允许你通过手动管理你的依赖关系，而无需使用CocoaPods或其他依赖关系管理器来管理依赖关系。 

以下是一些Carthage的命令：

- `update` - 用于更新或安装Cartfile或Cartfile.private中指定的所有依赖项。
- `bootstrap` - 在项目中生成一个Cartfile.resolved文件，其中包含所有必要的依赖项和版本信息。 这个文件可以被编译和上传到源代码控制管理器中，以便团队中的所有其他开发人员可以在项目的不同电脑上使用相同的依赖项版本。
- `build` - 构建一个或多个依赖项目。
- `archive` - 将指定依赖项构建为框架，并将其打包为.zip文件，可以将其分发给其他团队成员或作为可重用组件。
- `clean` - 清除构建文件和缓存文件夹。 

使用Carthage可以更加灵活地管理你的iOS项目的依赖项，但需要额外的手动管理。但是它比CocoaPods更加灵活和可定制，可以帮助你更好地控制你的iOS应用的构建和部署。 

## tldr 
 
> Cocoa 应用程序的依赖性管理工具。
> 更多信息：<https://github.com/Carthage/Carthage>.

- 下载 Cartfile 中提到的所有依赖项的最新版本，并编译它们：

`carthage update`

- 仅针对 IOS 平台，升级依赖文件：

`carthage update --platform ios`

- 仅更新依赖，但不编译它们：

`carthage update --no-build`

- 下载并重新生成依赖项的当前版本（不更新它们）：

`carthage bootstrap`

- 重新编译特定依赖项：

`carthage build {{依赖包}}`
