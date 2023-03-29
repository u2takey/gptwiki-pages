# alternatives 
## chatgpt 
alternatives是一个命令行工具，用于管理系统中存在的多个版本的类似软件的替代品。 

例如，在一个系统中可能会有多个Java版本，如JDK8、JDK11等。这些版本中的每一个都可以看作是Java的“替代版本”。alternatives工具允许用户轻松配置默认的Java版本，以及在不同的应用程序、脚本和用户之间切换Java版本。

使用alternatives的基本语法是：

```
alternatives [option...] <command>
```

该命令行工具通常使用一些常用选项，如： --display， --config，--install，--remove等。

下面是一些常用选项的解释：

- --display : 显示所有可用的备选项及其优先级；
- --config : 允许交互式修改和选择备选项的配置；
- --install : 安装备选项；
- --remove : 删除备选项;
- --auto : 将默认优先级分配给给定的备选项；
- --set : 设置给定备选项为默认选项。

以Java版本控制为例，下面是一些使用样例：

1. 显示所有可用Java版本的列表及其优先级：

```
$ alternatives --display java
```

2. 设置一个给定版本的Java为默认版本：

```
$ alternatives --set java /path/to/java-11/bin/java
```

3. 安装一个替代Java版本：

```
$ alternatives --install /usr/bin/java java /path/to/java-8/bin/java 2
```

4. 选择一个优先级较高的Java版本：

```
$ alternatives --auto java
```

以上是一些常见的alternatives命令的用法，该命令行工具也可以用于其他应用程序和软件的版本控制。 

## tldr 
 
> 这是 `update-alternatives` 命令的一个别名。
> 更多信息：<https://manned.org/alternatives>.

- 原命令的文档在：

`tldr update-alternatives`
