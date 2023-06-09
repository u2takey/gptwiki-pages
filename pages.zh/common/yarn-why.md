# yarn-why 
## chatgpt 
"yarn-why" 是 Yarn 工具的一个命令，用于分析为什么一个包（package）被安装在项目中。它会输出该包被安装的原因和依赖关系。

具体来说，yarn-why 命令会接收一个包名作为参数，然后遍历项目中的依赖树，找出所有依赖该包的原因，包括哪些依赖直接依赖该包，哪些依赖依赖了依赖该包的其他包等等。

此外，yarn-why 还可以接收一个可选参数，用于输出更详细的日志信息，帮助开发者更好地理解包的安装原因和依赖关系。

总之，yarn-why 命令是一个强大的分析工具，可以让开发者深入理解项目中的依赖关系，并进行复杂的依赖管理。 

## tldr 
 
> 确认安装这个 Yarn 软件包的原因。
> 更多信息：<https://github.com/amio/yarn-why>.

- 打印安装这个 Yarn 软件包的原因：

`yarn-why {{package_name}}`
