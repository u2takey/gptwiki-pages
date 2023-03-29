# ansible-playbook 
## chatgpt 
ansible-playbook 是一个命令行工具，用于运行 Ansible Playbook 任务。具体来说：

- ansible-playbook 用于在目标主机上运行 Ansible Playbook 任务。
- Ansible Playbook 是定义一系列操作步骤的文本文件，以自动执行在远程机器上的配置变更, 应用部署, 任务协调, 以及其他 IT 自动化任务。
- ansible-playbook 可以通过传递命令行选项和参数来自定义任务的执行和行为：例如定义目标主机、指定 Playbook 文件等等。
- ansible-playbook 是 Ansible 的核心组件之一，它支持自动化管理 Linux 和 Windows 系统，支持基于 SSH、WinRM、Powershell 等协议，使得操作系统配置与管理更加可靠、可重复且易于自动化。 

## tldr 
 
> 通过 SSH 协议在远程计算机上执行 playbook 中定义的任务。
> 更多信息：<https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

- 执行 playbook 中的任务：

`ansible-playbook {{playbook}}`

- 在给定的主机清单文件中执行 playbook 中的命令：

`ansible-playbook {{playbook}} -i {{清单文件}}`

- 通过定义在命令行中额外的变量执行 playbook 中的任务：

`ansible-playbook {{playbook}} -e "{{变量 1}}={{值 1}} {{变量 2}}={{值 2}}"`

- 通过定义在一个 json 格式的文件中额外的变量执行 playbook 中的任务：

`ansible-playbook {{playbook}} -e "@{{variables.json}}"`
