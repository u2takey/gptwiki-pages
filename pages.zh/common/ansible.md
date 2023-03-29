# ansible 
## chatgpt 
Ansible是一款开源的自动化IT工具，可以用来自动化部署、管理和配置计算机系统。ansible命令是用于运行Ansible工具的命令。

该命令的一些常见选项和参数包括：

- `-i`：指定Ansible所使用的主机清单文件。
- `-m`：指定要执行的模块。
- `-a`：指定模块所需的参数。
- `-u`：指定远程主机的用户名。
- `-k`：提示输入远程主机的密码。
- `-K`：提示输入sudo密码。
- `-f`：指定并发任务数。
- `-v`：增加日志级别，可以多次使用以增加详细程度。

例如，要使用ansible命令执行一个简单的命令，例如查看主机名：

```
ansible all -m command -a "hostname"
```

此命令将在所有主机上执行`hostname`命令并输出结果。如果您已经在Ansible主机上设置了SSH代理服务器，则可以使用以下命令：

```
ansible all -m ping
```

此命令将在所有主机上执行ping测试，以验证是否可以成功连接该主机。 

## tldr 
 
> 通过 SSH 协议远程管理计算机组。使用 `/etc/ansible/hosts` 文件来添加组 / 主机。
> 此命令也有关于其子命令的文件，例如：`ansible galaxy`.
> 更多信息：<https://www.ansible.com/>.

- 列出给定组下的所有主机：

`ansible {{组}} --list-hosts`

- 调用 ping 模块来 ping 一组主机：

`ansible {{组}} -m ping`

- 通过调用安装模块来显示关于一组主机的信息：

`ansible {{组}} -m setup`

- 调用命令模块并使用给定的参数来对一组主机执行命令：

`ansible {{组}} -m command -a '{{命令}}'`

- 以管理员权限执行一个命令：

`ansible {{组}} --become --ask-become-pass -m command -a '{{命令}}'`

- 使用自定义的清单文件执行一个命令：

`ansible {{组}} -i {{清单文件}} -m command -a '{{命令}}'`
