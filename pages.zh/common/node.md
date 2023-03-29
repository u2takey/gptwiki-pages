# node 
## chatgpt 
"node" 命令是一个在命令行界面下用于执行 JavaScript 代码的程序。简单来说，Node.js 是一个基于 Chrome V8 引擎的 JavaScript 运行环境，它使得我们可以使用 JavaScript 在服务器端运行代码、操作文件系统和进行网络通信等。

当运行 "node" 命令时，它会在命令行下打开一个 REPL（Read-Eval-Print Loop）环境，这是一个交互式的控制台环境，可以在其中逐行执行 JavaScript 代码。在 REPL 环境下，可以随时输入 JavaScript 代码，并立即看到其运行结果。

此外，"node" 命令还可以通过参数指定一个 JavaScript 文件的路径，让其在命令行下执行 JavaScript 文件的代码。例如，执行 "node app.js" 命令会运行名为 "app.js" 的 JavaScript 文件的代码。这种方式通常被用于在服务器端启动一个 Web 应用程序。

总而言之，"node" 命令是 Node.js 程序的入口点，使用它可以启动 Node.js 的 REPL 环境，或者执行指定 JavaScript 文件的代码。 

## tldr 
 
> 服务器后端 JavaScript 平台（Node.js）。
> 更多信息：<https://nodejs.org>.

- 运行一个 JavaScript 文件：

`node {{文件名}}`

- 开始一个 REPL 交互式解释器：

`node`

- 执行输入的 JavaScript 代码：

`node -e "{{代码}}"`

- 执行输入的 JavaScript 代码并显示结果：

`node -p "{{代码}}"`

- 启动检查器并在程序源码解析完成后等待调试器连接：

`node --no-lazy --inspect-brk {{文件名}}`
