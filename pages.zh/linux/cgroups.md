# cgroups 
## chatgpt 
cgroups（Control groups）是Linux内核中的一种资源分配和限制机制，可以用于控制和限制进程组、用户组或系统组使用CPU、内存、I/O等资源的量。它可以使系统管理员更好地控制系统资源的分配和使用，避免由于某个应用程序占用大量资源导致其他应用程序不能正常运行的问题。

cgroups 可以通过在/proc/cgroups 中创建一个层次结构来进行组织和管理。在这个层次结构中，每个组都可以被定义为一个子系统，并赋予不同的参数。cgroups 可以被视为虚拟容器，它们可以被动态地创建、销毁、合并和移动。

cgroups 在 Linux 中的应用非常广泛，包括容器技术，系统资源管理，虚拟机管理等领域。在命令行中，可以通过 cgcreate、 cgdelete、 cgexec、 cgclassify 等命令来创建、删除、运行和归类 cgroups。例如，要创建一个名为 mygroup 的 cgroup 并使用它来限制当前 shell 进程的 CPU 使用量，可以使用以下命令：

1.创建 cgroup：
sudo cgcreate -g cpu:/mygroup

2.将进程归类到 cgroup 中：
sudo cgclassify -g cpu:/mygroup $$

3.设定 cgroup 的 CPU 限制为最多使用 20% 的 CPU：
echo 20000 | sudo tee /sys/fs/cgroup/cpu/mygroup/cpu.cfs_quota_us

4.将进程移除 cgroup：
sudo cgclassify -g cpu:/mygroup $$

这样，当前 shell 进程就被限制在使用最多20%的 CPU上。以上是 cgroups 的简单示例，更多详细信息可以参考 Linux 各个发行版的官方文档或网络上的相关资料。 

## tldr 
 
> 这是 `cgclassify` 命令的一个别名。
> 更多信息：<https://www.kernel.org/doc/Documentation/cgroup-v2.txt>.

- 原命令的文档在：

`tldr cgclassify`
