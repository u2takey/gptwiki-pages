# etcd 
## chatgpt 
etcd是一个高可用的键值存储系统。它是用Go语言编写的，并且模仿了Google的Chubby的设计。etcd是一个分布式系统，可以用于分布式锁，分布式选举和服务注册与发现。它通过Raft算法保证数据安全性和一致性，并且提供对外的HTTP(S) API，用户可以通过API查询、设置、删除键值对，以及监控键值变化。

etcd的命令用于管理etcd集群。常用的命令如下：

- etcdctl endpoint health：检查etcd集群的健康状况。
- etcdctl member list：查看etcd集群中所有成员的信息。
- etcdctl put key value：在etcd集群中插入一个键值对。
- etcdctl get key：从etcd集群中获取指定键的值。
- etcdctl watch key：监视etcd集群中指定键的变化。
- etcdctl lease grant TTL：为etcd集群中的某个键生成一个租约，并指定过期时间。
- etcdctl snapshot save path：将etcd集群的快照保存到指定路径。

除了以上命令，etcd还有一些其他的管理命令，用户可以根据需要进行使用。 

## tldr 
 
> 分布式，可靠的键值存储，用于分布式系统中存储最关键的数据。
> 更多信息：<https://etcd.io>.

- 启动单节点 etcd 集群：

`etcd`

- 启动一个单节点 etcd 集群，在自定义 URL 上侦听客户端请求：

`etcd --advertise-client-urls {{http://127.0.0.1:1234}} --listen-client-urls {{http://127.0.0.1:1234}}`

- 使用自定义名称启动单节点 etcd 集群：

`etcd --name {{my_etcd_cluster}}`

- 启动单节点 etcd 集群，同时可以在这里看到大量监控指标 http://localhost:2379/debug/pprof/：

`etcd --enable-pprof --metrics extensive`
