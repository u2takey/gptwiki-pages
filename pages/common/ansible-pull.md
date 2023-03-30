# ansible-pull 
## chatgpt 
The `ansible-pull` command is an Ansible utility command that is used to run an Ansible playbook locally on the target machine. Unlike the typical Ansible usage, where Ansible connects to remote machines to execute tasks, `ansible-pull` runs the desired playbook on the local machine. This can be useful in several cases, such as:

- When you need a machine to configure itself based on a playbook stored in a central location such as a Git repository.
- When you want to run an ad-hoc playbook on a single machine without the need to install or configure Ansible on the local machine.

The `ansible-pull` command pulls the playbook from a remote source (e.g., Github, GitLab, or Bitbucket) and runs it locally on the target machine. Additionally, it can use Ansible's dynamic inventory to determine which host(s) the playbook should be run on. 

Here is an example of how to use `ansible-pull` to run a playbook from a remote Git repository:

```
ansible-pull -U https://github.com/myuser/my-playbook.git
```

This will pull the `my-playbook` project from the remote Git repository and execute it locally on the target machine.

You can also specify which playbook to run by providing the local file path or name of the playbook using the `-i` flag, such as:

```
ansible-pull -U https://github.com/myuser/my-playbook.git -i playbook.yml
```

This will pull the `my-playbook` project from the remote Git repository and execute the `playbook.yml` file located in the root directory of the project.

Overall, `ansible-pull` provides an easy and efficient way to run Ansible playbooks locally on a target machine, making it a valuable tool for local configurations and ad-hoc automation tasks. 

## tldr 
 
> Pull ansible playbooks from a VCS repo and executes them for the local host.
> More information: <https://docs.ansible.com/ansible/latest/cli/ansible-pull.html>.

- Pull a playbook from a VCS and execute a default local.yml playbook:

`ansible-pull -U {{repository_url}}`

- Pull a playbook from a VCS and execute a specific playbook:

`ansible-pull -U {{repository_url}} {{playbook}}`

- Pull a playbook from a VCS at a specific branch and execute a specific playbook:

`ansible-pull -U {{repository_url}} -C {{branch}} {{playbook}}`

- Pull a playbook from a VCS, specify hosts file and execute a specific playbook:

`ansible-pull -U {{repository_url}} -i {{hosts_file}} {{playbook}}`
