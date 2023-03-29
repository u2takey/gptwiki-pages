# a2ensite 
## chatgpt 
a2ensite是一个Linux命令，用于在Apache服务器上启用一个站点（也称为虚拟主机）。

具体而言，a2ensite命令会在Apache服务器的sites-enabled目录中创建一个软链接，将其链接到sites-available目录中对应站点的配置文件上。这个软链接的名称通常和对应站点的配置文件名称相同。

在使用a2ensite命令之后，当Apache服务器重新启动时，该站点就会被启用，并可以通过网站的域名或IP地址进行访问。

举个例子，如果要启用名为example.com的站点，可以使用以下命令：

a2ensite example.com

这会将sites-available/example.com文件链接到sites-enabled/example.com，从而启用该站点。 

## tldr 
 
> 在基于 Debian 的操作系统上启用 Apache 虚拟主机。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2ensite.8.en.html>.

- 启用虚拟主机：

`sudo a2ensite {{虚拟主机名}}`

- 不显示信息性消息：

`sudo a2ensite --quiet {{虚拟主机名}}`
