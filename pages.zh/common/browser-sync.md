# browser-sync 
## chatgpt 
browser-sync是一个用于自动化开发工作流的工具，它允许开发者在浏览器中实时地预览网站或应用程序，并自动刷新不同的浏览器中的页面。它具有以下特点：

1. 可以在本地创建服务器环境，并同步多个浏览器和设备中的应用程序和页面。

2. 可以自动刷新页面，以节省开发时间和提高生产力。

3. 可以在修改文件时自动编译SCSS、LESS等CSS预处理器、TypeScript等编程语言，以及自动刷新浏览器等功能。

4. 可以在实时编辑CSS或JavaScript时自动预览网站或应用程序效果。

命令行中运行以下命令，即可使用browser-sync工具：

browser-sync start [options]

其中，options中包含了的各种参数选项可以在命令行中使用，从而对工具进行配置，使其符合特定的需求和用例。常用的选项包括server、proxy、port、files、watch等等，详情可参考官方文档。 

## tldr 
 
> 启动一个本地的服务，可以监听文件改动，刷新浏览器。
> 更多信息：<https://browsersync.io/docs/command-line>.

- 将指定目录发成服务：

`browser-sync start --server {{路径/到/目录}} --files {{路径/到/目录}}`

- 启动当前目录服务，同时监听指定目录下 `css` 文件的变动：

`browser-sync start --server --files '{{路径/到/目录/*.css}}'`

- 创建配置文件：

`browser-sync init`

- 按指定配置文件中的配置启动服务：

`browser-sync start --config {{配置文件}}`
