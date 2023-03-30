# choco pack 
## chatgpt 
命令 "choco pack" 是 Chocolatey 包管理器中的一个命令，用于将软件或工具打包成 Chocolatey 包。打包后，可以将该包上传至 Chocolatey 社区仓库或者将其提供给自己的内部仓库供其他人员使用。在使用 choco pack 命令之前，用户需要创建一个包含有关软件和工具的元数据的本地文件夹。这个元数据包括有软件名称、版本、说明、安装脚本、卸载脚本等信息。choco pack 命令会读取元数据文件夹中的文件，并创建一个符合标准的 Chocolatey 包。这个命令的详细使用方法可以参考 Chocolatey 的官方文档。 

## tldr 
 
> 将 nuspec 打包到已编译的 nupkg.
> 更多信息：<https://chocolatey.org/docs/commands-pack>.

- 将 nuspec 打包到已编译的 nupkg：

`choco pack {{nuspec 的路径}}`

- 将 nuspec 打包到已编译的 nupkg, 并指定生成的版本：

`choco pack {{nuspec 的路径}} --version {{版本号}}`

- 将 nuspec 打包到已编译的 nupkg, 并输出到指定的目录：

`choco pack {{nuspec 的路径}} --output-directory {{输出目录的路径}}`
