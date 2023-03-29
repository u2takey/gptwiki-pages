# grub-mkconfig 
## chatgpt 
grub-mkconfig 是 Linux系统中GRUB（GRand Unified Bootloader）的一个命令，其作用是生成 GRUB 配置文件。GRUB是一款开源的多引导加载程序，允许用户选择启动哪个操作系统或者配置文件。

grub-mkconfig 命令会扫描 Linux系统 硬盘上的操作系统，并根据操作系统的类型、内核和其他相关信息自动生成 grub.cfg 配置文件。这个配置文件非常重要，它包含了诸如内核版本、分区信息、启动选项等所有启动操作系统的参数。

grub-mkconfig 命令的使用非常简单。只需要在 root 用户终端中执行以下命令即可生成 grub2 的配置文件：

```
# grub-mkconfig -o /boot/grub/grub.cfg
```

在命令行中输入以上命令，然后按下回车键。该命令将在 /boot/grub/grub.cfg 位置创建一个新的 grub 配置文件。

注：在执行此命令之前，必须先安装 GRUB，并将其设置为启动加载程序。另外，grub-mkconfig 命令较为复杂，需要根据具体的系统和需求进行不同的设置和参数调整。建议使用该命令前先了解 GRUB 的基本工作原理和相关配置文件的结构。 

## tldr 
 
> 生成GRUB配置文件。
> 更多信息：<https://www.gnu.org/software/grub/manual/grub/html_node/Invoking-grub_002dmkconfig.html>.

- 模拟运行并打印配置到标准输出：

`sudo grub-mkconfig`

- 生成配置文件：

`sudo grub-mkconfig --output={{/boot/grub/grub.cfg}}`

- 打印帮助页面：

`grub-mkconfig --help`
