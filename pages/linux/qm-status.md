# qm status 
## chatgpt 
The command "qm status" is used in the Proxmox environment to check the status of a virtual machine. When this command is executed, it provides information about the current state of the virtual machine, such as whether it is running, stopped, or in a suspended state.

Here is a breakdown of the output of the "qm status" command:

- If the machine is running, the output would show "status: running" and "uptime".
- If the machine is stopped, it would show "status: stopped" and the reason for the stop, either "exitstatus" or "gueststopped".
- If the machine is suspended, it would show "status: paused" and the reason why it was paused.

The qm status command also displays other information such as the machine’s ID, descriptions, memory consumption, and CPU usage.

Overall, the "qm status" command is a quick way to check the status of a virtual machine in Proxmox and helps in monitoring the virtual machine's health and performance. 

## tldr 
 
> Show virtual machine status.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Display the status of a specific virtual machine:

`qm status {{vm_id}}`

- Display detailed status of a specific virtual machine:

`qm status --verbose {{true}} {{vm_id}}`
