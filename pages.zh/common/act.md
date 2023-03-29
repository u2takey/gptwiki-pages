# act 
## chatgpt 
`act` 命令是一个基于 GitHub Actions 的命令行工具，它可以使用户更易于本地测试、构建和调试 GitHub Action 工作流程（workflows）。

该命令的基本用法为：

```
act [event] [options]
```

其中，`event` 为需要执行的事件名称，可以是本地存在的 GitHub Action 工作流程的名称也可通过 `-s` 参数指定一个 YAML 文件作为工作流程的定义；`options` 则为可选参数。根据不同的参数，`act` 命令可以执行不同的操作，例如：

- `--list`：列出可用的事件列表或工作流程列表；
- `--secret SECRET_NAME=SECRET_VALUE`：添加指定的 GitHub secrets；
- `-b BRANCH, --branch BRANCH`：指定要使用的 Git 分支；
- `--target TARGET`：指定要使用的模拟容器（默认为 Ubuntu 18.04）；
- `-j, --json`：以 JSON 格式输出结果；
- `-v, --verbose`：详细输出执行过程。

使用 `act` 命令可以让用户在本地快速测试和调试 GitHub Action 工作流程，从而在实际部署之前解决可能出现的问题，提高开发效率和代码质量。 

## tldr 
 
> 使用 Docker 本地运行 GitHub Actions.
> 更多信息：<https://github.com/nektos/act>.

- 列出可用的 actions 清单：

`act -l`

- 运行默认 event：

`act`

- 运行指定 event：

`act {{事件类型}}`

- 运行指定 action：

`act -a {{action_id}}`

- 非实际运行 actions（也就是 dry-run 模式）：

`act -n`

- 展示详细记录：

`act -v`
