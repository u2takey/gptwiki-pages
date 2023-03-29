# 7za 
## chatgpt 
7za是一个命令行工具，是7-Zip压缩和解压缩程序的一部分。它可以用于创建和提取7z，XZ，BZIP2，GZIP，TAR，ZIP，WIM和ISO文件格式。

下面列出了七个常用的参数选项解释：

1. a - 添加文件到存档文件中
2. x - 从存档文件中提取文件
3. e - 从存档文件中提取所有文件到当前目录
4. l - 列出存档文件的内容
5. t - 测试存档文件，检查文件是否完好无损
6. u - 更新存档文件，添加更新或新文件到存档文件中
7. d - 删除存档文件中指定的文件

其他选项包括：

-ai：指定档案名称。有时需要这个命令，以使7za能自动识别archive-type。如果书写错误的话， 将无法打压缩包。
-ax：指定排除列表的文件。
-o：指定提取文件的目录。 

## tldr 
 
> 一个高压缩率的文件归档器。
> 类似于 `7z`，支持的文档类型更少但跨平台。
> 更多信息：<https://www.7-zip.org>.

- 归档一个文件或目录：

`7za a {{归档文件.7z}} {{文件或目录}}`

- 加密一个已存在的归档文件（包括文件名）：

`7za a {{加密文件.7z}} -p{{密码}} -mhe=on {{归档文件.7z}}`

- 提取一个已存在的 7z 文件，并保持原来的目录结构：

`7za x {{归档文件.7z}}`

- 提取一个归档文件到指定目录：

`7za x {{归档文件.7z}} -o{{输出目录}}`

- 提取一个归档文件到标准输出：

`7za x {{归档文件.7z}} -so`

- 使用指定的类型来归档文件：

`7za a -t{{7z|bzip2|gzip|lzip|tar|zip}} {{归档文件.7z}} {{文件或目录}}`

- 列出一个归档文件的内容：

`7za l {{归档文件.7z}}`

- 列出可用的归档文件类型：

`7za i`