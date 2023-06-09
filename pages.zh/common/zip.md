# zip 
## chatgpt 
zip是一个用于压缩、打包和归档文件和目录的UNIX命令行工具。它能够将多个文件和目录打包成一个文件，而这个文件可以压缩或者未压缩，常用于备份或传输数据。

zip命令包含多个选项和参数，以下是常用的选项和参数：

-options：用于设置选项，例如-r表示递归地压缩目录中的所有文件，-q表示“安静”模式（即不显示处理进度）。
-file.zip：用于指定输出的ZIP文件的名称。
file：要压缩的文件或目录的名称。

以下是几个常用的示例：
1. 压缩文件：zip file.zip file1.txt file2.txt

2. 压缩目录及其中的所有文件：zip -r dir.zip directory/

3. 将压缩文件解压缩到指定目录：unzip file.zip -d directory/

4. 将压缩文件中的文件列表打印到屏幕：unzip -l file.zip

需要注意的是，zip命令只能用于UNIX环境中，而在Windows环境中，需要使用WinZip或其他类似软件。 

## tldr 
 
> 将文件打包并压缩（存档）为 zip 文件。
> 更多信息：<https://manned.org/zip>.

- 递归地打包和压缩文件和目录：

`zip -r {{压缩文件.zip}} {{路径/到/文件}} {{路径/到/目录1}} {{路径/到/目录2}}`

- 添加到压缩档案中并排除不需要的文件：

`zip -r {{压缩文件.zip}} {{路径/到/目录}} -x {{路径/到/不需要的文件}}`

- 使用最高压缩级别 9 压缩目录和内容：

`zip -r -{{9}} {{压缩文件.zip}} {{路径/到/目录}}`

- 创建一个加密压缩档案（将会提示输入密码）：

`zip -e -r {{压缩文件.zip}} {{路径/到/目录}}`

- 将文件添加到现有的 zip 文件：

`zip {{压缩文件.zip}} {{路径/到/文件}}`

- 从现有 zip 文件中删除文件：

`zip -d {{压缩文件.zip}} "{{foo/*.tmp}}"`

- 将指定目录及其内容打包并拆分为多个 zip 文件（例如：若干个 3 GB 的 zip 包）：

`zip -r -s {{3g}} {{压缩文件.zip}} {{路径/到/目录}}`

- 列出指定压缩档案中的文件（不提取文件）：

`zip -sf {{压缩文件.zip}}`
