# pacstrap 
## chatgpt 
`pacstrap` is a command in Arch Linux used to install essential packages for a base installation of the operating system. It is used during the installation process to create a new system using the Arch Linux installation media.

The command is used as follows:

```pacstrap /mnt base```

What it does:

- `pacstrap` is the command that installs packages.
- `/mnt` is the target directory where the packages will be installed. In most cases, this is the root directory.
- `base` is a package group that includes everything needed for a basic Arch Linux installation, including the Linux kernel, network tools, and basic utilities.

Additional options:

- `--needed` flag: Only install packages that are not already installed.
- `--ignore` flag: Ignore packages that you don't want to be installed.
- `-c` flag: Use the specified cache directory instead of the default one.
- `-G` flag: Include packages from base-devel group.
- `-i` flag: Install the package from a local package file.
- `-M` flag: Include and install all packages from the specified mirror.

Once you run the `pacstrap` command, it will start downloading and installing the packages needed for a basic Arch Linux installation in your target directory. The time it takes to complete the command will depend on your internet connection and the speed of your computer. 

## tldr 
 
> Arch Linux install script to install packages to the specified new root directory.
> More information: <https://man.archlinux.org/man/pacstrap.8>.

- Install the `base` package, Linux kernel and firmware for common hardware:

`pacstrap {{path/to/new/root}} {{base}} {{linux}} {{linux-firmware}}`

- Install the `base` package, Linux LTS kernel and `base-devel` build tools:

`pacstrap {{path/to/new/root}} {{base}} {{base-devel}} {{linux-lts}}`

- Install packages without copy the host's mirrorlist to the target:

`pacstrap -M {{path/to/new/root}} {{packages}}`

- Use an alternate configuration file for Pacman:

`pacstrap -C {{path/to/pacman.conf}} {{path/to/new/root}} {{packages}}`

- Install packages using the package cache on the host instead of on the target:

`pacstrap -c {{path/to/new/root}} {{packages}}`

- Install packages without copy the host's pacman keyring to the target:

`pacstrap -G {{path/to/new/root}} {{packages}}`

- Install packages in interactive mode (prompts for confirmation):

`pacstrap -i {{path/to/new/root}} {{packages}}`

- Install packages using package files:

`pacstrap -U {{path/to/new/root}} {{path/to/package1}} {{path/to/package2}}`
