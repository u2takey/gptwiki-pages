# apt-file 
## chatgpt 
apt-file是Linux系统中一个命令行工具，可以用来查找软件包中特定文件的名称和位置。它在Debian和Ubuntu等Linux发行版中使用。

使用apt-file命令需要安装apt-file软件包，然后运行以下命令进行初始化：

```
sudo apt-file update
```

这将下载软件包列表，以便apt-file可以比较这些列表并查找特定的文件。接下来，您可以使用apt-file命令来查找软件包中特定文件的位置。例如，您可以使用以下命令来查找一个名为“foo”的文件：

```
apt-file search foo
```

这将列出包含“foo”文件的所有可用软件包。如果您想查找特定软件包中的文件，请运行以下命令：

```
apt-file list packagename
```

这将列出指定软件包中的所有文件。apt-file命令非常实用，可帮助您快速查找软件包中的文件，特别是需要安装新软件包时。 

## tldr 
 
> 在 apt 软件包中查找文件，其中也包括未安装的软件。
> 更多信息：<https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

- 更新元数据的数据库：

`sudo apt update`

- 查找包含指定文件或路径的软件包：

`apt-file {{search|find}} {{文件路径}}`

- 列出指定包的内容：

`apt-file {{show|list}} {{软件包名}}`

- 查找符合给定 `pattern` 中正则表达式的软件包：

`apt-file {{search|find}} --regexp {{正则表达式}}`
