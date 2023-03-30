# grub-reboot 
## chatgpt 
The `grub-reboot` command is a Linux utility used to set the default boot entry for the next boot. This command allows the system administrator to specify which operating system or kernel to boot into without having to manually select it at startup.

When executed, the `grub-reboot` command takes a numerical argument, which corresponds to the order in which the entries are listed in the GRUB bootloader. For example, if the first entry on the GRUB menu is "Ubuntu", and the second entry is "Windows", running the command `grub-reboot 2` will set the system to boot Windows on the next startup.

It is important to note that the `grub-reboot` command only sets the default boot entry for the next boot. After the system is restarted or shut down, the default boot entry will be reset to its original setting. To permanently change the default boot entry, users can modify the GRUB configuration file (/etc/default/grub) or use the `update-grub` command.

Overall, the `grub-reboot` command is a powerful tool for managing dual-boot systems or testing different operating systems or kernels. 

## tldr 
 
> Set the default boot entry for GRUB, for the next boot only.
> More information: <https://manned.org/grub-reboot>.

- Set the default boot entry to an entry number, name or identifier for the next boot:

`sudo grub-reboot {{entry_number}}`

- Set the default boot entry to an entry number, name or identifier for an alternative boot directory for the next boot:

`sudo grub-reboot --boot-directory {{/path/to/boot_directory}} {{entry_number}}`
