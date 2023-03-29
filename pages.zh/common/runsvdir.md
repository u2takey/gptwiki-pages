# runsvdir 
## chatgpt 
runsvdir是一个运行sv程序的守护进程，它会监视一个目录（通常是/etc/service），并启动每个服务目录中的run程序。runsvdir命令的详细解释如下：

1. 语法

runsvdir [选项] [目录]

2. 选项

- --help：显示帮助消息；
- --version：显示版本信息；
- --supervised：以监控模式运行；
- --chdir <目录>：切换到指定目录并运行。

3. 参数

- 目录：要监视的服务目录，默认为/etc/service。

4. 描述

runsvdir是一个守护进程，它会监视一个目录中的子目录，并启动每个子目录中的run程序。runsvdir通常用于运行服务，例如网络服务、应用程序等，它能够自动启动、停止和重新启动服务。

runsvdir使用的服务目录通常是/etc/service，但也可以通过命令行参数指定其他目录。该目录中应该包含每个服务的子目录，每个子目录中包含一个名为run的可执行文件，以及其他必要的文件和配置文件。

runsvdir会通过调用run程序来启动每个服务，每个服务的输出将被记录到该服务目录中的log目录下的相应日志文件中。runsvdir还会为每个服务生成一个PID文件，方便管理和控制服务。

5. 示例

要运行runsvdir以监视默认的服务目录/etc/service并启动其中的所有服务，可以使用以下命令：

runsvdir /etc/service

要以监控模式运行runsvdir，可以使用以下命令：

runsvdir --supervised /etc/service

此时，如果某个服务停止运行，runsvdir会自动重新启动该服务。

要指定监视的服务目录，可以使用以下命令：

runsvdir --chdir /opt/services /opt/services

此命令将目录/opt/services作为服务目录，并在该目录中启动所有服务。 

## tldr 
 
> 运行整个目录下的服务。
> 更多信息：<https://manpages.ubuntu.com/manpages/latest/man8/runsvdir.8.html>.

- 以当前用户身份启动和管理目录中的所有服务：

`runsvdir {{目录 / 服务文件}}`

- 以 root 用户身份启动和管理目录中的所有服务：

`sudo runsvdir {{目录 / 服务文件}}`

- 在单独会话中启动服务：

`runsvdir -P {{目录 / 服务文件}}`
