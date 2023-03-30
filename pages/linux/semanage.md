# semanage 
## chatgpt 
semanage is a command-line utility that can be used to manage SELinux-related policies on a Linux-based system. It allows system administrators to view and modify SELinux policies and permissions in a more granular and fine-tuned manner.

Some of the main functions of semanage include modifying SELinux policy rules for file contexts, ports, booleans, users, roles, and types. It also allows administrators to control network access, configure SELinux modules, and troubleshoot common SELinux issues.

For example, using the semanage command, you can adjust file contexts for directories and files, which determines how access control policies are applied to them. You can also modify port contexts to allow specific network traffic to pass through, or enable/disable SELinux booleans to grant or deny extra permissions to users.

Overall, semanage is a versatile and powerful tool that can provide advanced control over SELinux policies on a Linux system. However, it requires a solid understanding of SELinux concepts and policies to be used effectively. 

## tldr 
 
> SELinux Policy Management tool.
> More information: <https://manned.org/semanage>.

- Output local customizations:

`semanage -S {{store}} -o {{path/to/output_file}}`

- Take a set of commands from a specified file and load them in a single transaction:

`semanage -S {{store}} -i {{path/to/input_file}}`

- Manage booleans. Booleans allow the administrator to modify the confinement of processes based on the current configuration:

`semanage boolean -S {{store}} {{--delete|--modify|--list|--noheading|--deleteall}} {{-on|-off}} -F {{boolean|boolean_file}}`

- Manage policy modules:

`semanage module -S {{store}} {{--add|--delete|--list|--modify}} {{--enable|--disable}} {{module_name}}`

- Disable/Enable dontaudit rules in policy:

`semanage dontaudit -S {{store}} {{on|off}}`
