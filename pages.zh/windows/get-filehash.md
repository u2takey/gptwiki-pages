# Get-FileHash 
## chatgpt 
Get-FileHash 是 PowerShell 的一个命令，它用于获取文件的哈希值。哈希值是通过对文件内容应用哈希算法计算得出的一串字符，可以用于验证文件的完整性和唯一性。

使用 Get-FileHash 命令时，需要指定要计算哈希值的文件的路径，可以使用绝对路径或者相对路径。

Get-FileHash 命令支持多种哈希算法，包括 MD5、SHA1、SHA256、SHA384 和 SHA512。可以通过指定 -Algorithm 参数来选择要使用的哈希算法。例如：

Get-FileHash -Path "C:\temp\myfile.txt" -Algorithm MD5

以上命令会计算指定文件的 MD5 哈希值。

Get-FileHash 命令还支持在输出中包含计算出的哈希值的算法和文件路径等信息。可以使用 -Algorithm 和 -LiteralPath 参数来控制输出的信息。例如：

Get-FileHash -Path "C:\temp\myfile.txt" -Algorithm SHA256 | Format-List

以上命令会计算指定文件的 SHA256 哈希值，并以详细信息的格式输出。 

## tldr 
 
> 计算一个文件的 HASH 值。
> 更多信息：<https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash>.

- 使用 SHA256 算法计算给定文件的哈希值：

`Get-FileHash {{文件路径}}`

- 使用指定的哈希算法计算给定文件的哈希值：

`Get-FileHash {{文件路径}} -Algorithm {{SHA1|SHA384|SHA256|SHA512|MD5}}`
