# efibootmgr 
## chatgpt 
The "efibootmgr" command is used to manage the boot entries stored in the EFI (Extensible Firmware Interface) firmware of a computer. This command can be executed from a terminal or command prompt in Linux-based operating systems.

Some of the common options/arguments used with "efibootmgr" command are:

1. "-v" or "--verbose" - displays detailed information about the boot entries.
2. "-o" or "--bootorder" - sets the boot order of the boot entries.
3. "-d" or "--disk" - specifies the disk device for which the boot entries are managed.
4. "-p" or "--part" - specifies the partition number on the disk device to access the EFI system partition.
5. "-c" or "--create" - creates a new boot entry.
6. "-t" or "--timeout" - sets the timeout value for the boot menu in seconds.
7. "-B" or "--delete-bootnum" - deletes a boot entry based on its boot number.

Using "efibootmgr" command, users can add or remove boot entries, change boot order, set a default boot entry, and even rename entries. This command is particularly useful in multi-boot setups where users need to switch between different operating systems installed on the same machine. 

## tldr 
 
> Manipulate the UEFI Boot Manager.
> More information: <https://manned.org/efibootmgr>.

- List the current settings then bootnums with their name:

`efibootmgr`

- List the filepaths:

`efibootmgr -v`

- Add UEFI Shell v2 as a boot option:

`sudo efibootmgr -c -d {{/dev/sda1}} -l {{\EFI\tools\Shell.efi}} -L "{{UEFI Shell}}"`

- Change the current boot order:

`sudo efibootmgr -o {{0002,0008,0001,0005}}`

- Delete a boot option:

`sudo efibootmgr -b {{0008}} --delete-bootnum`
