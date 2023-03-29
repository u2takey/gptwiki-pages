# gpg 
## chatgpt 
gpg( GNU Privacy Guard)是一个加密软件，常用于保护文件的安全性。它可以用于加密、解密、签名和验证文件或通信内容。

以下是gpg常用的命令：

1. gpg --encrypt 文件名：用默认的加密算法加密文件。

2. gpg --decrypt 文件名：用默认的加密算法解密文件。

3. gpg --sign 文件名：使用你的私钥给文件签名。

4. gpg --verify 文件名：验证文件的签名是否有效。

5. gpg --gen-key ：创建RSA和DSA私钥对和一个公钥。

6. gpg --export：将公钥导出到文件，使其他人可以使用它来加密消息。

7. gpg --import：从文件中导入公钥。

8. gpg --list-keys：列出所有已安装的密钥。

9. gpg --delete-key 密钥ID：删除一个特定的密钥。

10. gpg --edit-key 密钥ID：修改密钥属性。

11. gpg --export-secret-keys：导出私钥到文件。

12. gpg --delete-secret-key 密钥ID：删除私钥。

注意：使用gpg命令需要谨慎操作。任意使用或不小心保护密钥可能会导致数据丢失或泄漏。因此，请在使用gpg之前，确保你已经充分了解其功能和使用方法，并保证密钥的安全存储。 

## tldr 
 
> GNU Privacy Guard.
> 请参阅`gpg2`了解 GNU Privacy Guard 2.
> 更多信息：<https://gnupg.org>.

- 不加密，仅对`doc.txt`进行签名（生成`doc.txt.asc`，格式为 ASCII 码形式）：

`gpg --clearsign {{doc.txt}}`

- 对`doc.txt`进行签名并加密（生成`doc.txt.asc`，格式为 ASCII 码形式）：

`gpg --local-user {{sender_id}} --recipient {{recipient_id}} --armor --sign --encrypt {{doc.txt}}`

- 为接收者 alice@example.com 加密`doc.txt`（生成`doc.txt.gpg`）：

`gpg --encrypt --recipient {{alice@example.com}} {{doc.txt}}`

- 只用密码加密`doc.txt`（生成`doc.txt.gpg`）：

`gpg --symmetric {{doc.txt}}`

- 解密`doc.txt.gpg`（输出到标准输出）：

`gpg --decrypt {{doc.txt.gpg}}`

- 导入一个公钥：

`gpg --import {{public.gpg}}`

- 导出 alice@example.com 的公钥（输出到标准输出）：

`gpg --export --armor {{alice@example.com}}`

- 导出 alice@example.com 的私钥（输出到标准输出）：

`gpg --export-secret-keys --armor {{alice@example.com}}`
