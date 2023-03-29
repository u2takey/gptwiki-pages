# gpgv 
## chatgpt 
gpgv是一个用于验证数字签名的GNU隐私保护（GnuPG）工具之一。它通常用于验证软件包签名或颁发者的签名，以确保数据的完整性和真实性。具体来说，gpgv从文件中读取数字签名，然后检查它是否与附加到文件中的实际数据匹配。如果签名是有效的，则gpgv返回零（成功），否则返回非零值（失败）。

gpgv工具的基本格式如下：

gpgv [--keyring filename] [--status-fd n] [--logger-fd n] [--ignore-time] [--max-output n] [-o file] [-r keyid] file [file ...]

其中：

- --keyring：指示要使用的公钥文件，默认为系统的主密钥环。
- --status-fd：指示消息和状态信息的输出描述符。默认输出到标准错误流（stderr）。
- --logger-fd：指示日志信息的输出描述符。默认输出到标准错误流。
- --ignore-time：指示忽略签名时间的时间戳检查。这意味着已经过期的签名也会被接受。默认情况下，gpgv会检查签名是否在指定的时间段内有效。
- --max-output：指示最大输出量（以字节为单位）。超过此限制的输出将被截断。默认为4096字节。
- -o：指示将验证结果输出到指定文件中，而不是标准输出（stdout）。
- -r：指示使用给定的密钥ID验证签名。如果未指定此选项，则gpgv将尝试使用系统中找到的密钥进行验证。
- file：必需参数，指示要验证的文件。

通过gpgv命令进行数字签名验证是一项重要的安全措施，可以确保软件包和其他数据不被篡改或变造。 

## tldr 
 
> 验证 OpenPGP 签名。
> 更多信息：<https://www.gnupg.org/documentation/manuals/gnupg/gpgv.html>.

- 验证签名文件：

`gpgv {{path/to/file}}`

- 使用分离式签名验证已签名的文件：

`gpgv {{path/to/signature}} {{path/to/file}}`

- 在 keyrings 列表中添加一个文件（一个导出的钥匙也算作一个 keyring）：

`gpgv --keyring {{path/to/keyring_file}} {{path/to/signature}} {{path/to/file}}`
