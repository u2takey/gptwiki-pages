# rustfmt 
## chatgpt 
rustfmt是一个rust的代码格式化工具。它可以将您的代码转换为符合Rust编程规范和惯例的格式。您可以使用rustfmt命令，将您的代码通过控制台传递给rustfmt进行格式化。

rustfmt的一些用途包括：

1. 自动格式化您的代码，以符合Rust代码约定和规范。
2. 帮助您减少代码错误，特别是在您需要更改代码结构时，例如调整缩进和添加新的数据结构。
3. 在代码提交到版本控制系统（如Git）之前，使用rustfmt检查代码格式化错误。

rustfmt有多个选项可以使用，包括：

1. --help 显示rustfmt命令的帮助信息。
2. --check 如果有任何错误，将退出并返回非零值。
3. --write-mode 表示在原有文件上更改格式。如果文件不能被更改，将会在格式化后生成一个新文件。

例如，为了格式化一个Rust模块，您可以使用以下命令：

```
rustfmt mod.rs
```

该命令将读取mod.rs文件，并将其格式化为符合Rust编程规范和惯例的格式。

需要注意的是，rustfmt并不是唯一的Rust代码格式化工具，您也可以使用其他工具（例如Clippy和Rust语言服务器）来帮助您格式化代码。 

## tldr 
 
> 格式化 Rust 源代码的工具。
> 更多信息：<https://github.com/rust-lang/rustfmt>.

- 格式化文件，就地覆盖原始文件：

`rustfmt {{路径/到/源文件.rs}}`

- 检查文件的格式并在控制台上显示所有更改：

`rustfmt --check {{路径/到/源文件.rs}}`

- 格式化之前，备份所有修改过的文件（原始文件的扩展名为 `.bk`）：

`rustfmt --backup {{路径/到/源文件.rs}}`
