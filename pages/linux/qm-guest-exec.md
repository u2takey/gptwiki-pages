# qm guest exec 
## chatgpt 
The "qm guest exec" command is a command-line utility used in the Proxmox virtualization environment to execute a command within a virtual machine. 

The "qm" part of the command refers to the QEMU Machine, which is the virtual machine manager used by Proxmox. 

The "guest" part of the command specifies that the command will be executed within a virtual machine. 

The "exec" part of the command specifies that a command will be executed within the virtual machine.

To use this command, you will need to provide the ID of the virtual machine that you want to execute the command in, as well as the actual command to be executed. The syntax for the command is as follows:

qm guest exec <vmid> <command>

Where <vmid> is the ID of the virtual machine you want to execute the command in, and <command> is the command you want to execute within the virtual machine.

For example, to execute the command "ls -l" within virtual machine 100, you would run the following command:

qm guest exec 100 ls -l

Note that this command can only be run while logged in as the root user on the Proxmox server. Additionally, the virtual machine must be running in order for the command to be executed. 

## tldr 
 
> Execute a specific command via a guest agent.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Execute a specific command via a guest agent:

`qm guest exec {{vm_id}} {{command}} {{arg1 arg2 ...}}`

- Execute a specific command via a guest agent asynchronously:

`qm guest exec {{vm_id}} {{arg1 arg2 ...}} --synchronous 0`

- Execute a specific command via a guest agent with a specified timeout of 10 seconds:

`qm guest exec {{vm_id}} {{arg1 arg2 ...}} --timeout {{10}}`

- Execute a specific command via a guest agent and forward input from STDIN until EOF to the guest agent:

`qm guest exec {{vm_id}} {{arg1 arg2 ...}} --pass-stdin 1`
