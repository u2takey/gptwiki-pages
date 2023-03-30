# gtr 
## chatgpt 
gtr是一个Linux和Unix shell的命令，用于比较两个字符串或两个文件中的文本。

语法：
gtr [OPTION]… SET1 [SET2]

参数及选项：

SET1：要比较的第一个字符集
SET2：要比较的第二个字符集

选项：
-c：按照字符顺序比较,以ASCII值为序
-d：比较十进制数字，忽略非数字字符
-i：对大小写不敏感
-u：比较十进制数字，忽略非数字字符

示例：

1.比较两个字母

$ echo a b | gtr a b
b a

2.将字符转换为大写

$ echo "abcdefg" | gtr 'a-z' 'A-Z'
ABCDEFG

3.比较两个文件

$ gtr -d "\n" < file1.txt > file2.txt
此命令将file1.txt中的每个换行符替换为十进制数字，并将输出写入file2.txt中。
 

## tldr 
 
> 这是 `-p linux tr` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux tr`
