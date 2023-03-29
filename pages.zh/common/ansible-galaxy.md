# ansible-galaxy 
## chatgpt 
ansible-galaxy 是 Ansible 官方提供的一个命令行工具，用于管理 Ansible roles（角色）的工具，它可以让管理员非常方便地查找、下载、安装和分享 Ansible roles。

ansible-galaxy 命令有以下常用子命令：

- init：在当前目录下创建一个新的 role；

- search：通过关键字在 galaxy.ansible.com 上搜索 roles；

- install：安装已经存在于 Ansible Galaxy 上的 role；

- remove：移除已安装的 role；

- import：将一个包含 role 的压缩文件导入到 Ansible Galaxy 中；

- list：显示已安装的 role 列表。

使用 ansible-galaxy 命令，可以方便地发现其他人编写的 roles，不管是在个人博客、GitHub 还是在 Ansible Galaxy 平台中，都可以通过命令查找、保存、管理 roles。它是 Ansible 中的一个方便且非常强大的工具。 

## tldr 
 
> 创建和管理 Ansible 角色。
> 更多信息：<https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

- 安装一个角色：

`ansible-galaxy install {{用户名.角色名}}`

- 移除一个角色：

`ansible-galaxy remove {{用户名.角色名}}`

- 列出已安装的角色：

`ansible-galaxy list`

- 搜索一个指定的角色：

`ansible-galaxy search {{角色名}}`

- 创建一个新的角色：

`ansible-galaxy init {{角色名}}`
