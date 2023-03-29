# poweroff 
## chatgpt 
Linux命令poweroff是一个用于关闭系统的命令，当用户执行该命令时，系统将立即关闭并关闭计算机。该命令使用root用户权限执行。

该命令的具体行为取决于系统的配置和硬件，例如关闭计算机后是否自动重新启动。在执行poweroff命令之前，用户应该确保所有正在进行的程序都已保存并关闭，以避免数据丢失。

poweroff命令可以通过以下方式执行：

```
sudo poweroff
```

或者

```
su -c "poweroff"
```

需要注意的是，执行该命令将直接关闭计算机，因此在执行该命令之前，应该谨慎考虑并确保所有操作都已保存。 

## tldr 
 
> 关闭系统。
> 更多信息：<https://www.man7.org/linux/man-pages/man8/poweroff.8.html>.

- 关闭系统电源：

`sudo poweroff`
