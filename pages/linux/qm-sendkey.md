# qm sendkey 
## chatgpt 
The command "qm sendkey" refers to the function of sending keyboard input to a virtual machine hosted on a Linux-based server. The "qm" part stands for "qemu machine," which is the name of a popular open-source virtualization program used to run multiple operating systems on a single physical machine.

When you send a "key" using this command, you are essentially simulating the act of typing on a keyboard within the virtual machine's console or graphical interface. This can be useful in a variety of scenarios, such as when you need to enter commands or keystrokes that are not easily accessible through other means.

The "sendkey" part of the command specifies what type of keyboard input to send to the virtual machine. You can use various options to specify the exact character or sequence of characters you want to send, such as "ctrl-alt-del" to simulate the pressing of the Control, Alt, and Delete keys at once.

Overall, the qm sendkey command is an important tool for managing virtual machines and automating routine tasks that would otherwise require manual intervention. It allows you to control virtual machines from the command line, and can help streamline your workflow when working with virtualized environments. 

## tldr 
 
> Send QEMU monitor encoding key event to a virtual machine.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Send the specified key event to a specific virtual machine:

`qm sendkey {{vm_id}} {{key}}`

- Allow root user to send key event and ignore locks:

`qm sendkey --skiplock {{true}} {{vm_id}} {{key}}`
