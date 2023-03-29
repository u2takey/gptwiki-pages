# sacctmgr 
## chatgpt 
sacctmgr是一个用于管理Slurm的命令行工具，Slurm是一个开源的分布式资源管理和调度系统，用于管理大量计算机集群资源。sacctmgr可以管理帐户、分区、节点、集群等多种资源。

使用sacctmgr可以执行以下操作：

1. 创建和管理帐户

使用sacctmgr可以创建和删除帐户，还可以将帐户添加到或删除自己管理的分区或群集。

2. 创建和管理分区

sacctmgr可以创建和删除分区，也可以将分区添加到或从自己管理的群集中删除。

3. 创建和管理节点

使用sacctmgr可以向群集中添加或删除计算节点，还可以将节点分配给一个或多个分区。

4. 管理现有的集群

通过sacctmgr，管理员可以监视和管理集群资源的使用情况，包括节点、核心和内存消耗情况。

5. 管理配额和限制

使用sacctmgr可以设置和修改帐户、分区和节点的配额和限制，以限制资源使用量。

总的来说，sacctmgr是一个非常强大的工具，用于管理Slurm系统中的各种资源，可以有效地管理大型计算机集群，提高计算机系统的资源利用率。 

## tldr 
 
> 查看、配置、管理 Slurm 账户。
> 更多信息：<https://slurm.schedmd.com/sacctmgr.html>.

- 显示现有配置：

`sacctmgr show configuration`

- 向 Slurm 数据库添加集群：

`sacctmgr add cluster {{集群名}}`

- 向 Slurm 数据库添加账户：

`sacctmgr add account {{账户名}} cluster={{账户所在集群}}`

- 以指定格式显示用户、账户资源关联、集群、账户的详细信息：

`sacctmgr show {{user|association|cluster|account}} format="Accout%10" format="GrpTRES%30"`
