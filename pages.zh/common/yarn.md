# yarn 
## chatgpt 
yarn是一个用于管理前端项目依赖关系的工具，类似于npm。

以下是yarn的一些常用命令：

1. yarn init - 初始化一个新的yarn软件包并生成一个package.json文件
2. yarn install - 安装所有npm依赖项
3. yarn add [package] - 安装一个新的依赖项 package
4. yarn remove [package] -移除一个依赖项package
5. yarn upgrade [package] -更新一个依赖项package
6. yarn run [script] - 运行在package.json中定义的脚本

其他常见的yarn命令还包括yarn cache、yarn global、yarn link等。

yarn也有一些高级功能，比如支持离线模式，可以提高项目的构建效率。它还可以与其他工具（比如Webpack和Babel）集成，以提供更强大的功能。 

## tldr 
 
> JavaScript 和 Node.js package manager 的一个替代。
> 更多信息：<https://yarnpkg.com>.

- 全局安装一个模块：

`yarn global add {{module_name}}`

- 安装 `package.json` 中指定的依赖（`install` 命令是可选的 -- 你可以直接输入`yarn`）：

`yarn install`

- 安装一个模块并将其写入 `package.json` 中的依赖项（增加 `--dev` 来作为开发依赖写入）：

`yarn add {{module_name}}@{{version}}`

- 卸载一个模块并将其从 `package.json` 的依赖项中移除：

`yarn remove {{module_name}}`

- 交互式地创建一个 `package.json` 文件：

`yarn init`

- 确认一个模块是否是一个依赖项并且列出依赖其的模块：

`yarn why {{module_name}}`
