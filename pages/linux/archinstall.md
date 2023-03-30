# archinstall 
## chatgpt 
The `archinstall` is a command-line tool used in the Arch Linux operating system. It is a streamlined and simplified installer for Arch Linux designed to quickly and easily set up a complete operating system environment.

When executed, the `archinstall` command process leads the user through a series of questions and prompts to customize their installation, such as selecting the language, time zone, and keyboard layout. 

The `archinstall` command can also be used to perform a completely automated installation of Arch Linux, known as the "headless" setup mode, by creating its own configuration file. In this mode, the installer will use the specified configuration file to automatically complete the installation process without user intervention, making it an efficient way to deploy applications in a production environment. 

The `archinstall` tool has the following features:

- Supports different partitions and file systems, including the Btrfs and ZFS file systems.
- Ability to manage advanced disk encryption.
- Power to configure kernel parameters and install additional packages during the installation process
- Ability to create a user account and set passwords for it during the installation process.

Overall, `archinstall` streamlines the installation of Arch Linux, making it a useful tool for both home and enterprise users. 

## tldr 
 
> Guided Arch Linux installer with a twist.
> More information: <https://archinstall.readthedocs.io>.

- Start the interactive installer:

`archinstall`

- Start a preset installer:

`archinstall {{minimal|unattended}}`
