# qm guest cmd 
## chatgpt 
The "qm guest cmd" command is a command-line interface (CLI) command used in Proxmox Virtual Environment (PVE) to execute commands within a guest virtual machine (VM). 

Breaking down the command:

- "qm" stands for "Qemu Manager", which is the management tool used to manage virtual machines in PVE.
- "guest" refers to a specific guest VM in PVE.
- "cmd" is short for "command", which is the action we want to execute within the guest VM.

Usage:

To use the "qm guest cmd" command, you first need to know the ID (numeric identifier) of the guest VM you want to run the command in. Once you have that information, you can run the following command:

```
qm guest cmd <vmid> <command>
```

where:
- "vmid" is the ID of the guest VM you want to run the command in.
- "command" is the command you want to execute within the guest VM.

For example, to run the command "ls -l" (which lists the contents of a directory in a long format) within guest VM with ID 100, you would run the following command:

```
qm guest cmd 100 'ls -l'
```

Note that the command to be executed within the guest VM needs to be enclosed in quotes.

Security consideration:

The "qm guest cmd" command should be used with caution, as it provides direct access to the guest VM's file system and could potentially be used to compromise the security of the system. Only trusted users should be given permission to execute this command. Additionally, it is recommended to use SSH keys rather than passwords for authentication when executing guest commands remotely. 

## tldr 
 
> Execute QEMU Guest Agent commands.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Execute a specific QEMU Guest Agent command:

`qm guest cmd {{virtual_machine_id}} {{fsfreeze-freeze|fsfreeze-status|fsfreeze-thaw|fstrim|get-fsinfo|...}}`
