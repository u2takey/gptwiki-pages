# rubocop 
## chatgpt 
Rubocop是一个Ruby代码风格指南和自动修复工具。它基于Ruby社区的风格指南并提供了一系列检查规则，可以帮助开发者遵循一致的风格，提高代码的可读性和维护性。

运行Rubocop命令后，它会分析当前项目中所有Ruby文件，并提供有关代码风格和最佳实践的一系列警告和建议。这些警告包括不规范的缩进、空格、变量命名、代码复杂度等问题。而建议则是关于改进代码质量和可读性的建议。

Rubocop还提供了自动修复功能，可以自动修复被警告的代码问题。可以在命令后面使用`--auto-correct`选项来启用该功能。

使用Rubocop可以帮助开发者遵循一致的代码风格，减少代码中的错误和不规范，提高代码质量。 

## tldr 
 
> 格式化 Ruby 文件。
> 更多信息：<https://docs.rubocop.org/rubocop/usage/basic_usage.html>.

- 检查当前目录中的所有文件（包括子目录）：

`rubocop`

- 检查一个或多个指定文件或目录：

`rubocop {{目录 / 文件名}} {{目录 /}}`

- 将输出写入指定文件：

`rubocop --out {{目录 / 文件名}}`

- 查看规则列表（格式化规则）：

`rubocop --show-cops`

- 排除格式规则：

`rubocop --except {{规则 1}} {{规则 2}}`

- 只运行指定的规则：

`rubocop --only {{规则 1}} {{规则 2}}`

- 自动更正文件（实验）：

`rubocop --auto-correct`
