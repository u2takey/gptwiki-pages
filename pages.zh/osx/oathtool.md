# oathtool 
## chatgpt 
oathtool是一个命令行工具，用于生成和验证基于时间的一次性密码（TOTP）和基于哈希的一次性密码（HOTP）。

以下是一些常见用法：

1. 生成基于时间的一次性密码（TOTP）：

```
oathtool --base32 --totp "MY_SECRET_KEY"
```

其中，`MY_SECRET_KEY`是你的密钥，可以是任何字符串，如你的账户密码。

此命令将生成一个6位数字的TOTP密码，每30秒刷新一次。

2. 生成基于哈希的一次性密码（HOTP）：

```
oathtool --base32 --hotp "MY_SECRET_KEY" 0
```

其中，`MY_SECRET_KEY`是你的密钥，可以是任何字符串，如你的账户密码。`0`是计数器值，表示在该计数器值下生成一次性密码。

此命令将生成一个6位数字的HOTP密码。

3. 验证一次性密码：

```
oathtool --base32 --totp "MY_SECRET_KEY" --check "123456"
```

其中，`MY_SECRET_KEY`是你的密钥，可以是任何字符串，如你的账户密码。`123456`是你想要验证的密码。

此命令将验证给定的密码是否是当前有效的一次性密码。

除了上述用法外，oathtool还支持许多其他选项和用法，具体可以使用`man oathtool`命令查看文档。 

## tldr 
 
> OATH 一次性密码工具。

- 生成 TOTP 令牌（行为类似于 Google Authenticator）：

`oathtool --totp --base32 {{密码}}`

- 根据给定时间产生特定的 TOTP 令牌：

`oathtool --totp --now {{2004-02-29 16:21:42}} --base32 {{密码}}`

- 验证 TOTP 令牌：

`oathtool --totp --base32 {{密码}} {{令牌}}`
