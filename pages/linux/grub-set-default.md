# grub-set-default 
## chatgpt 
Grub-set-default is a command in Linux systems that is used to set the default boot entry in the GRUB (GRand Unified Bootloader) configuration file. It allows users to choose which operating system kernel or operating system version is loaded when their computer boots up.

The command works by modifying the grub configuration file (typically located in /boot/grub/grub.conf or /etc/default/grub) and changing the value of the DEFAULT parameter. The DEFAULT parameter specifies the default menu entry, and the number that it is set to corresponds to the order in which the entries appear in the GRUB menu.

To use the command, you need to specify the menu entry number that you want to set as the default. For example, if you want to set the second menu entry as the default, you would run the following command:

```
sudo grub-set-default 2
```

This would set the second entry as the default, and the system would boot up with that entry the next time the computer restarts. You can use the grub-editenv command to check the current default entry:

```
sudo grub-editenv list
```

The output of this command will show you the current value of the DEFAULT parameter, which should match the menu entry number that you set with grub-set-default.

Note that changes made with grub-set-default will only take effect after a system restart. Also, if you update or modify the GRUB configuration file, any changes made with grub-set-default may be overwritten. If you want to make permanent changes to the GRUB configuration file, you should edit the file directly rather than using this command. 

## tldr 
 
> Set the default boot entry for GRUB.
> More information: <https://manned.org/grub-set-default>.

- Set the default boot entry to an entry number, name or identifier:

`sudo grub-set-default {{entry_number}}`

- Set the default boot entry to an entry number, name or identifier for an alternative boot directory:

`sudo grub-set-default --boot-directory {{/path/to/boot_directory}} {{entry_number}}`
