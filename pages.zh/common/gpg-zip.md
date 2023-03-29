# gpg-zip 
## chatgpt 
gpg-zip 是 GnuPG（GNU隐私保护软件）中的一个工具，用于将文件或目录压缩并加密成一个 gpg 文件。使用 gpg-zip 命令时，可以通过指定参数来控制压缩和加密的过程。

以下是 gpg-zip 命令的常用参数：

- -c, --create：创建 gpg 文件
- -z, --gzip：使用 GZIP 压缩格式进行压缩
- -a, --armor：生成 ASCII 编码的 gpg 文件
- -e, --encrypt：加密生成的 gpg 文件
- -r, --recipient：指定加密使用的密钥
- -u, --local-user：指定使用的用户 ID

例如，下面的命令将压缩文件夹 /home/user/Documents，使用 GZIP 格式压缩，生成一个加密的 gpg 文件，并指定使用名为 test 的密钥进行加密，然后输出至 /home/user/Desktop：

```
gpg-zip -c -z -e -r test -o /home/user/Desktop/Documents.gpg /home/user/Documents
```

执行完毕后，系统将提示你输入加密使用的密钥密码。输入正确的密码之后，将生成一个加密的 gpg 文件，只有指定的密钥持有人才能解密进入该文件并查看其内容。 

## tldr 
 
> 使用`GPG`加密存档中的文件和目录。
> 更多信息：<https://www.gnupg.org/documentation/manuals/gnupg/gpg_002dzip.html>.

- 使用密码将一个目录加密为`archive.gpg`：

`gpg-zip --symmetric --output {{archive.gpg}} {{path/to/directory}}`

- 将`archive.gpg`解密到同名目录中：

`gpg-zip --decrypt {{path/to/archive.gpg}}`

- 列出加密的`archive.gpg`的内容：

`gpg-zip --list-archive {{path/to/archive.gpg}}`
