# grub-install 
## chatgpt 
Grub-install is a command used to install the GRUB (Grand Unified Bootloader) boot loader on a disk. The GRUB boot loader is responsible for loading the operating system and initiating the boot process.

The command typically requires superuser or administrative privileges to be executed. It needs to be run in a terminal or a console as a superuser using the sudo command. 

The syntax for the grub-install command is as follows:

```
grub-install [OPTION]... [--modules=MODULE]... INSTALL_DEVICE
```

Here, INSTALL_DEVICE refers to the device or partition where you want to install the GRUB boot loader. It can be a hard disk, a USB drive, or any other storage device. 

The following are some of the options that are commonly used with the grub-install command:

- `--force`: This option forces the installation of GRUB, even if the system's firmware does not support it.
- `--recheck`: This option rechecks the device map file and updates any changes that have been made since the last time that GRUB was installed.
- `--boot-directory=DIR`: This option specifies the directory containing the GRUB boot files. By default, this is the /boot/grub/ directory.
- `--grub-setup=/BIN/GRUB-SETUP`: This option allows the path to grub-setup to be specified to execute the setup portion of grub-install.

The grub-install command installs the GRUB boot loader on the master boot record (MBR) or the partition boot sector of the specified device. It also creates various configuration files and necessary directories under the /boot/grub/ directory.

Overall, the grub-install command is a powerful tool for managing boot loaders and can be incredibly useful for system administrators who need to manage multiple systems. 

## tldr 
 
> Install GRUB to a device.
> More information: <https://www.gnu.org/software/grub/manual/grub/html_node/Installing-GRUB-using-grub_002dinstall.html>.

- Install GRUB on a BIOS system:

`grub-install --target={{i386-pc}} {{path/to/device}}`

- Install GRUB on an UEFI system:

`grub-install --target={{x86_64-efi}} --efi-directory={{path/to/efi_directory}} --bootloader-id={{GRUB}}`

- Install GRUB pre-loading specific modules:

`grub-install --target={{x86_64-efi}} --efi-directory={{path/to/efi_directory}} --modules="{{part_gpt part_msdos}}"`
