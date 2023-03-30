# bootctl 
## chatgpt 
The "bootctl" command is used to manage the boot loader on Linux systems. The boot loader is the software responsible for loading the operating system kernel into memory so that it can be started up.

The "bootctl" command is typically used to manage the systemd-boot boot loader that is included in many Linux distributions. It allows you to view and modify the boot configuration, configure the boot options, and troubleshoot boot issues.

Here are some of the common options for the "bootctl" command:

- "status": This displays the status of the boot loader and any available boot entries.
- "list": This displays a list of all the available boot entries.
- "default": This sets the default boot entry.
- "set-oneshot": This sets a one-time boot option that will be used only for the next boot.
- "update": This updates the boot configuration with any changes made to it.

Overall, the "bootctl" command is a powerful tool for managing the boot loader on Linux systems. It can help you troubleshoot boot issues and customize the boot process to meet your particular needs. 

## tldr 
 
> Control EFI firmware boot settings and manage boot loader.
> More information: <https://manned.org/bootctl>.

- Show information about the system firmware and the bootloaders:

`sudo bootctl status`

- Set a flag to boot into the system firmware on the next boot (similar to `sudo systemctl reboot --firmware-setup`):

`sudo bootctl reboot-to-firmware true`

- Specify the path to the EFI system partition (defaults to `/efi/`, `/boot/` or `/boot/efi`):

`sudo bootctl --esp-path={{/path/to/efi_system_partition/}}`

- Show all available bootloader entries:

`sudo bootctl list`

- Install `systemd-boot` into the EFI system partition:

`sudo bootctl install`

- Remove all installed versions of `systemd-boot` from the EFI system partition:

`sudo bootctl remove`
