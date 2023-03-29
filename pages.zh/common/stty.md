# stty 
## chatgpt 
stty命令用于在终端设置和显示终端行设置。它控制多种终端和操作系统上的终端驱动程序和TTY设备，包括终端字符大小写、回显、ICANON、iterminal特性等。

常见用法参数：

- -a: 显示所有终端设置
- -g: 显示当前终端设置的字符串格式
- erase xxx: 设置终端退格键为XXX
- intr xxx: 设置终端中断键（通常是Ctrl+C）为XXX
- kill xxx: 设置终端终止键（通常是Ctrl+X）为XXX
- cooked: 设置终端为正常模式（会将终端缓冲中的数据写到文件中）
- raw: 设置终端为raw模式（不会将缓冲中的数据写到文件中）
- -echo: 关闭回显

例如：

```shell
# 查看终端设置
stty -a

# 将终端中断键设置为Ctrl+Z
stty intr ^Z

# 将回车转义为\n
stty icrnl

# 关闭回显
stty -echo
``` 

## tldr 
 
> 设置终端设备接口的选项。
> 更多信息：<https://www.gnu.org/software/coreutils/stty>.

- 显示当前终端的所有设置：

`stty -a`

- 设置行数：

`stty rows {{行数}}`

- 设置列数：

`stty cols {{列数}}`

- 获取设备的实际传输速度：

`stty -F {{目标 / 文件夹 / 驱动设备文件}} speed`

- 将当前终端的所有模式重置为合理值：

`stty sane`
