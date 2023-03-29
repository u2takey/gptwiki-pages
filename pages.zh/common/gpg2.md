# gpg2 
## chatgpt 
gpg2是一个加密和数字签名软件，是GNU Privacy Guard的一部分。gpg2允许用户创建和管理密钥，使用这些密钥加密和解密文件，并对文件进行数字签名和验证。下面是一些常用的gpg2命令：

1. gpg2 --gen-key: 创建GPG密钥对

2. gpg2 --import file: 导入外部公钥文件

3. gpg2 --export "name": 导出指定名称的公钥

4. gpg2 --list-keys: 列出所有公钥

5. gpg2 --list-secret-keys: 列出所有私钥

6. gpg2 --encrypt file: 用公钥加密文件

7. gpg2 --decrypt file.gpg: 用私钥解密加密文件

8. gpg2 --sign file: 对文件进行数字签名

9. gpg2 --verify file.sig: 验证数字签名

10. gpg2 --clearsign file: 清晰文本签名文件

11. gpg2 --armor: 将输出转换为ASCII格式

12. gpg2 --delete-key "name": 删除指定名称的密钥

需要注意的是，这里列出的命令可能不是所有的命令，如果您需要了解更多细节信息，可以查看gpg2的手册。 

## tldr 
 
> GNU Privacy Guard 2.
> GNU Privacy Guard 1 请参见`gpg`.
> 更多信息：<https://docs.releng.linuxfoundation.org/en/latest/gpg.html>.

- 列出导入的密钥（公钥）：

`gpg2 --list-keys`

- 为指定的接收者加密指定的文件，将输出结果写到一个新的文件中，并附加 `.gpg`：

`gpg2 --encrypt --recipient {{alice@example.com}} {{path/to/doc.txt}}`

- 只用密码（对称加密）对指定文件进行加密，将输出结果写入一个附加`.gpg`的新文件：

`gpg2 --symmetric {{path/to/doc.txt}}`

- 解密指定的文件，并将结果写入标准输出：

`gpg2 --decrypt {{path/to/doc.txt.gpg}}`

- 导入一个公钥：

`gpg2 --import {{path/to/public_key.gpg}}`

- 将指定电子邮件地址的公钥导出到标准输出：

`gpg2 --export --armor {{alice@example.com}}`

- 将指定电子邮件地址的私钥导出到标准输出：

`gpg2 --export-secret-keys --armor {{alice@example.com}}`
