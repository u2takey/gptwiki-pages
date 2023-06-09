# age 
## chatgpt 
age 命令是一个用于查看系统中所有用户最后登录时间的命令。当运行 age 命令时，它将扫描系统中所有用户的最后登录时间，并将其显示出来。如果用户在一定时间内没有登录过系统，系统会自动将其账户设置为过期或锁定，以增加系统的安全性。使用 age 命令可以方便地查看哪些用户最近活跃，并有助于管理员监控和管理系统的安全和稳定性。以下是用法示例：

用法：age [选项]...

选项：
  -d，--debug         调试模式
  -h，--help          显示帮助信息并退出
  -q，--quiet         安静模式
  -t，--threshold=天数    设置最后登录时间的阈值
  -u，--user=用户名      只显示指定用户的信息
  -V，--version       显示版本信息并退出

示例：
1. 显示所有用户的最后登录时间：
  age
2. 显示指定用户的最后登录时间：
  age -u username
3. 只显示最近7天登录过的用户：
  age -t 7
4. 安静模式，只显示用户列表，不显示其他信息：
  age -q
5. 显示版本信息：
  age -V 

## tldr 
 
> 一个简单、现代、安全的文件加密工具。
> 更多信息：<https://age-encryption.org>.

- 生成一个可以用密码短语（passphrase）解密的加密文件：

`age --passphrase --output {{路径/到/已加密文件}} {{路径/到/未加密文件}}`

- 生成一个密钥对，将私钥保存到一个未加密的文件，并将公钥打印到标准输出：

`age-keygen --output {{路径/到/文件}}`

- 用一个或多个公钥加密一个文件，这些公钥以字面形式输入：

`age --recipient {{公钥_1}} --recipient {{公钥_2}} {{路径/到/未加密文件}} --output {{路径/到/已加密文件}}`

- 用收件人文件中指定的一个或多个公钥来加密一个文件：

`age --recipients-file {{路径/到/收件人文件}} {{路径/到/未加密文件}} --output {{路径/到/已加密文件}}`

- 用密码短语解密一个文件：

`age --decrypt --output {{路径/到/已解密文件}} {{路径/到/已加密文件}}`

- 用私钥文件解密一个文件：

`age --decrypt --identity {{路径/到/私钥文件}} --output {{路径/到/已解密文件}} {{路径/到/已加密文件}}`
