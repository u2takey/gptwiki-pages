# gsha512sum 
## chatgpt 
命令名称：gsha512sum

命令功能：该命令是用于计算和校验SHA512散列值的命令行工具。SHA512是一种密码哈希函数，用于将数据转换为散列值或摘要，以便用于密码验证或数据完整性检查。

命令用法：gsha512sum [文件路径...]

选项说明：
- b / --binary：使用二进制模式计算散列值。
- s / --status：仅输出校验结果，不输出散列值。
- c / --check：用于校验已经存在的文件的散列值。
- t / --text：使用文本模式计算散列值。

命令示例：
1. 计算文件的SHA512散列值：gsha512sum file.txt
2. 将计算后的散列值存入文件：gsha512sum file.txt > hash.txt
3. 校验文件散列值是否与给定的散列值匹配：gsha512sum -c hash.txt

注意：使用gsha512sum命令时，应注意文件路径和文件名的正确性。如果文件名或路径不正确，则会产生错误。 

## tldr 
 
> 这是 `-p linux sha512sum` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sha512sum`
