# gping 
## chatgpt 
gping是一种可视化的ping工具，它可以在命令行或者终端中展示ping测试所得到的结果，包括每个测试的往返时间、时间统计、丢包率等信息。gping还可以显示每个ping测试的地理位置，这对于评估网络性能和网络故障排除非常有用。gping的另一个特点是它可以在图形界面中展示ping测试结果，这使得用户更容易理解测试结果并可通过图示方式比较测试结果。 gping命令的一些常用参数：

-g,--graphical：在图形用户界面中显示gping的结果

-H,--host：设置要ping的远程主机的主机名或IP地址。

-p, --port：设置远程主机的ping端口号。默认是80端口。

-S, --source：设置要使用的源地址。默认是本地IP地址。

-t, --ttl：设置ping的生存时间的初始值（TTL值）。默认是64。

-c, --count：设置要发送的ping包的数量。在无限循环模式下设置为0。

-i, --interval：设置间隔ping包之间的时间间隔（以毫秒为单位）。默认是1000ms。

-w, --wait：设置每个ping包的超时时间（以毫秒为单位）。默认是1000ms。

--help：显示gping命令的使用帮助。 

## tldr 
 
> 这是 `-p linux ping` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux ping`
