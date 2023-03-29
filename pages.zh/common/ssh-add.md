# ssh-add 
## chatgpt 
ssh-add是用于管理SSH私钥的命令行工具，它可以将私钥加入到ssh-agent的密钥缓存中。当您第一次连接到远程主机时，ssh-add可以让您避免在每次进行身份验证时输入SSH密码。

具体来说，ssh-add有以下用途：

1. 将SSH私钥添加到ssh-agent的密钥缓存中，免去在登录远程主机时反复输入密码的麻烦。

2. 列出ssh-agent已缓存的私钥列表。

3. 从ssh-agent密钥缓存中删除私钥。

4. 从ssh-agent密钥缓存中清除所有私钥。

使用ssh-add的基本语法如下：

$ ssh-add [OPTIONS] [IDENTITY_FILE]

其中IDENTITY_FILE是您要添加或删除的SSH私钥，可以是绝对路径或相对路径。如果不指定IDENTITY_FILE，则ssh-add会将默认的SSH私钥（即当前用户的~/.ssh/id_rsa）添加到ssh-agent的密钥缓存中。

常用的ssh-add命令行选项包括：

1. -l：列出ssh-agent已缓存的所有私钥。

2. -d：从ssh-agent密钥缓存中删除指定的私钥。

3. -D：从ssh-agent密钥缓存中清除所有私钥。

4. -t LIFE：指定ssh-agent中缓存私钥的超时时间，单位为秒。默认值为0，表示私钥不过期。

总之，ssh-add是SSH中非常重要且实用的工具，可以提高用户的工作效率和安全性。 

## tldr 
 
> 在 ssh 代理中管理加载的 ssh 密钥。
> 需要确保 ssh 代理已启动并正在运行以加载其中的密钥。
> 更多信息：<https://man.openbsd.org/ssh-add>.

- 将 `~/.ssh` 中的默认 ssh 密钥添加到 `ssh` 代理：

`ssh-add`

- 向 ssh 代理添加指定密钥：

`ssh-add {{目录 / 私钥文件}}`

- 列出当前加载的密钥的指纹：

`ssh-add -l`

- 从 ssh 代理中删除密钥：

`ssh-add -d {{目录 / 私钥文件}}`

- 从 ssh 代理中删除所有当前已有的密钥：

`ssh-add -D`

- 向 ssh 代理和密钥链添加密钥：

`ssh-add -K {{目录 / 私钥文件}}`
