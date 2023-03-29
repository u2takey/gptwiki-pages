# aurvote 
## chatgpt 
很抱歉，我作为AI语言模型无法详细解释"aurvote"命令，因为Linux系统中没有这个命令。也可能是您输入错误或打错了命令。请检查拼写或查阅相关文档以获取正确的命令信息。 

## tldr 
 
> 为 AUR 中的包投票。
> 为了投票成功，文件 `~/.config/aurvote` 必须存在并包含你的 AUR 身份凭证。
> 更多信息：<https://github.com/archlinuxfr/aurvote>.

- 交互式创建包含你的 AUR 用户名和密码的 `~/.config/aurvote` 文件：

`aurvote --configure`

- 为一个或多个 AUR 包投票：

`aurvote {{package1 package2 ...}}`

- 为一个或多个 AUR 包取消投票：

`aurvote --unvote {{package1 package2 ...}}`

- 检查一个或多个 AUR 包是否已投票：

`aurvote --check {{package1 package2 ...}}`

- 查看 `aurvote` 的帮助信息：

`aurvote --help`
