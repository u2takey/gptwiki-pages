# opkg 
## chatgpt 
Opkg is a package management tool designed for embedded systems like routers, wireless access points, and other devices that use Linux-based firmware. It is similar to the Advanced Packaging Tool (APT) used in Debian Linux distributions.

Opkg allows users to install, uninstall, and upgrade software packages on their embedded devices. The opkg command is used to interact with the package manager and perform various tasks like searching, installing, updating, and removing packages.

Here are some common opkg commands:

1. opkg update - This command updates the package list on the device by connecting to the repository server.

2. opkg install package_name - This command installs a package, where package_name is the name of the package you want to install.

3. opkg remove package_name - This command removes a package, where package_name is the name of the package you want to remove.

4. opkg upgrade - This command upgrades all installed packages to their latest version.

5. opkg list - This command lists all available packages on the repository server.

Opkg also supports various options that can be used with these commands to customize their behavior, such as --force-depends or --force-overwrite. It is important to understand the options and usage of each command before using them to ensure that the desired actions are taken on the device. 

## tldr 
 
> A lightweight package manager used to install OpenWrt packages.
> More information: <https://openwrt.org/docs/guide-user/additional-software/opkg>.

- Install a package:

`opkg install {{package}}`

- Remove a package:

`opkg remove {{package}}`

- Update the list of available packages:

`opkg update`

- Upgrade all the installed packages:

`opkg upgrade`

- Upgrade one or more specific package(s):

`opkg upgrade {{package(s)}}`

- Display information for a specific package:

`opkg info {{package}}`

- List all the available packages:

`opkg list`
