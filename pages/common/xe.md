# xe 
## chatgpt 
The "xe" command is a Linux command-line interface tool that is used to manage and control virtual machines running on a Xen hypervisor. It is a part of the XenServer management tool stack.

Here are some of the common options and actions that can be performed with the "xe" command:

- "xe vm-list": This command lists all the virtual machines running on the XenServer.
- "xe template-list": Lists all the available templates that can be used to create virtual machines.
- "xe host-list": Shows the list of all the hosts that are managed by the XenServer.
- "xe vm-start": This command is used to start a specified virtual machine.
- "xe vm-shutdown": Shuts down a specified virtual machine gracefully.
- "xe vm-reboot": Reboots a specified virtual machine.
- "xe vm-snapshot": Creates a snapshot of the specified virtual machine.
- "xe vm-export": Exports a specified virtual machine to a file that can be used to import the virtual machine to another XenServer.

Overall, the "xe" command is a powerful tool that allows users to manage, monitor and control virtual machines running on a Xen hypervisor. 

## tldr 
 
> Execute a command once for each line piped from another command or file.
> More information: <https://github.com/leahneukirchen/xe>.

- Run a command once for each line of input data as arguments:

`{{arguments_source}} | xe {{command}}`

- Execute the commands, replacing any occurrence of the placeholder (marked as `{}`) with the input line:

`{{arguments_source}} | xe {{command}} {} {{optional_extra_arguments}}`

- Execute a shellscript, joining every `N` lines into a single call:

`echo -e 'a\nb' | xe -N{{2}} -s 'echo $2 $1'`

- Delete all files with a `.backup` extension:

`find . -name {{'*.backup'}} | xe rm -v`

- Run up to `max-jobs` processes in parallel; the default is 1. If `max-jobs` is 0, xe will run as many processes as cpu cores:

`{{arguments_source}} | xe -j {{max-jobs}} {{command}}`
