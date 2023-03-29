# hostname 
## chatgpt 
`hostname` 命令是用于显示或设置系统的主机名称（或计算机名）。主机名是一个用来区分网络上不同计算机的文本标识符。它通常由一个主机名和一个域名组成，格式如下：`hostname.domain.com`。

以下是该命令常用的选项：

- `-a`：显示所有的别名
- `-d`：仅显示域名
- `-f`：显示完全限定域名（FQDN）
- `-i`：显示主机的IP地址
- `-s`：仅显示主机名，不包括域名
- `-v`：显示版本信息
- `-h` 或 `--help`：显示帮助信息。

例如，要设置主机名称为 `myhost`，可以使用以下命令：

```
hostname myhost
```

要显示当前主机名和完全限定域名，可以使用以下命令：

```
hostname
``` 

## tldr 
 
> 显示或设置系统的主机名。
> 更多信息：<https://manned.org/hostname>.

- 显示本机的主机名：

`hostname`

- 设置本机主机名：

`hostname {{新主机名}}`