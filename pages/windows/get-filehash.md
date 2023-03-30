# Get-FileHash 
## chatgpt 
The `Get-FileHash` command is a PowerShell command that generates a hash value for a file. A hash value is a unique code that represents the contents of a file in a short alphanumeric format. This code is generated using a cryptographic hashing algorithm which produces a fixed-length string of characters that is unique to the input. It is used to verify file integrity, and to ensure that the file has not been tampered with or corrupted.

The syntax for the `Get-FileHash` command is as follows:

```
Get-FileHash [-Path] <String[]> [-Algorithm <String>] [-LiteralPath <String[]>] [-Stream <String>] [<CommonParameters>]
```

- `-Path`: Specifies the path of the file to be hashed. This parameter is required.
- `-Algorithm`: Specifies the hashing algorithm to be used. The default is SHA256, but other options include SHA1, SHA384, SHA512, and MD5.
- `-LiteralPath`: Specifies the path of the file to be hashed, without any wildcard characters. This parameter is useful when dealing with files that have special characters in their names.
- `-Stream`: Specifies the name of an alternate data stream to be hashed. This parameter is used when working with files that have more than one data stream.

Once you have executed the command, `Get-FileHash` will calculate the hash value for the specified file, using the specified algorithm. The output will include the hash value, the algorithm used, and the file name. 

The `Get-FileHash` command can help you verify the integrity of a file by comparing its hash value to a known hash value. If the hash values match, then it is likely that the file has not been modified. If they do not match, then it is possible that the file has been tampered with or corrupted. 

## tldr 
 
> Calculate a hash for a file.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash>.

- Calculate a hash for a specified file using the SHA256 algorithm:

`Get-FileHash {{path\to\file}}`

- Calculate a hash for a specified file using a specified algorithm:

`Get-FileHash {{path\to\file}} -Algorithm {{SHA1|SHA384|SHA256|SHA512|MD5}}`
