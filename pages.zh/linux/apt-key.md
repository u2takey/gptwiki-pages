# apt-key 
## chatgpt 
apt-key是Debian/Ubuntu系统中的一个命令，用于管理系统中的软件包密钥。软件包密钥是用于验证软件包和存储库的数字签名的标识符。

该命令主要用于以下操作：

1.添加密钥：可以从特定存储库中获取公共密钥，并将其添加到系统中，以验证相关软件包的数字签名。

2.删除密钥：可以删除已经添加到系统中但不再需要的密钥。

3.列出密钥：可以列出系统中已添加的所有密钥。

例如，要添加一个密钥，可以使用以下命令：

```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 40976EAF437D05B5
```

该命令将从 Ubuntu 密钥服务器获取公共密钥并将其添加到系统中。

要删除一个密钥，可以使用以下命令：

```
sudo apt-key del 40976EAF437D05B5
```

该命令将从系统中删除指定的密钥。

要列出已添加的所有密钥，可以使用以下命令：

```
sudo apt-key list
```

该命令将列出系统中所有已添加的密钥，并显示每个密钥的ID和名称。 

## tldr 
 
> Debian 和 Ubuntu 上的 APT 软件包管理器的密钥管理工具。
> 更多信息：<https://manpages.debian.org/latest/apt/apt-key.8.html>.

- 列出可信密钥：

`apt-key list`

- 向可信密钥库中添加一个密钥：

`apt-key add {{密钥文件.asc}}`

- 从可信密钥库中移除一个密钥：

`apt-key del {{密钥 id}}`

- 向可信密钥库中添加一个远程密钥：

`wget -qO - {{https://host.tld/filename.key}} | apt-key add -`

- 指定密钥 ID, 从密钥服务器中添加一个密钥：

`apt-key adv --keyserver {{pgp.mit.edu}} --recv {{密钥 id}}`
