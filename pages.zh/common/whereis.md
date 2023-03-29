# whereis 
## chatgpt 
`whereis`是一个Linux命令，用于查找指定程序、命令的二进制文件位置、源代码文件位置、帮助文档位置。

具体使用方法如下：

语法：whereis [命令] 

选项： 
- -b：查找可执行文件位置 
- -m：查找帮助文档位置 
- -s：查找源代码文件位置 

示例：输入命令“whereis ls”将返回ls命令的二进制文件位置和帮助文档位置。输入命令“whereis -s ls”返回ls命令的源代码文件位置。 

## tldr 
 
> 找到命令的二进制，源文件和手册文件。
> 更多信息：<https://manned.org/whereis>.

- 找到 `ssh` 命令的二进制、源文件和手册页：

`whereis {{ssh}}`

- 查找 `ls` 命令的二进制和手册页：

`whereis -bm {{ls}}`

- 找到 `gc` 的源文件和 `git` 的手册页：

`whereis -s {{gcc}} -m {{git}}`

- 仅在 /usr/bin/ 目录中查找 `gcc` 的二进制文件：

`whereis -b -B {{/usr/bin/}} -f {{gcc}}`
