# a2enconf 
## chatgpt 
a2enconf 是一个用于在 Apache2 中启用配置文件的命令。该命令会将指定的配置文件从 Apache2 的 /etc/apache2/conf-available 目录中链接到 /etc/apache2/conf-enabled 目录下，使其能够被 Apache2 所加载。

a2enconf 有两种用法：

1. 使用文件名启用单个配置文件：

```
a2enconf conf-name
```

其中，conf-name 为被启用的配置文件的文件名（不含扩展名）。

2. 使用通配符启用多个配置文件：

```
a2enconf conf-*
```

其中，conf-* 为符合条件的配置文件通配符。该命令会启用 /etc/apache2/conf-available 目录中所有以 conf- 开头的配置文件。

需要注意的是，a2enconf 仅用于启用配置文件，如果想要禁用配置文件，需要使用 a2disconf 命令。该命令的用法与 a2enconf 相似，只不过是将配置文件从 /etc/apache2/conf-enabled 目录中删除。 

## tldr 
 
> 在基于 Debian 的操作系统上启用 Apache 配置文件。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2enconf.8.en.html>.

- 启用配置文件：

`sudo a2enconf {{配置文件}}`

- 不显示信息性消息：

`sudo a2enconf --quiet {{配置文件}}`
