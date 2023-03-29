# anbox 
## chatgpt 
anbox是一个开源框架，可以在Linux系统中运行安卓应用程序。它提供了一个虚拟安卓环境，其中安卓应用程序可以像常规Linux应用程序一样运行。通过anbox，用户可以在Linux系统中使用安卓应用程序，而无需使用模拟器或虚拟机。

anbox命令是用于启动和管理anbox的命令。可以使用该命令来启动anbox会话，列出已安装的应用程序，安装新的应用程序，启动已安装的应用程序等。以下是一些常用的anbox命令：

1. anbox session-manager：启动anbox会话管理器。

2. anbox launch --package=[包名] --activity=[活动名]：启动指定的安卓应用程序。需要指定应用程序的包名和活动名。

3. anbox install [应用程序路径]：安装指定路径下的安卓应用程序。

4. anbox list-installed：列出已安装的安卓应用程序。

5. anbox uninstall [包名]：卸载指定的安卓应用程序。需要指定应用程序的包名。

通过以上命令，用户可以启动、管理anbox会话，并在其中运行安卓应用程序。 

## tldr 
 
> 在任何 GNU/Linux 操作系统上运行安卓应用。
> 更多信息：<https://manned.org/anbox>.

- 在应用管理器中运行 Anbox：

`anbox launch --package={{org.anbox.appmgr}} --component={{org.anbox.appmgr.AppViewActivity}}`
