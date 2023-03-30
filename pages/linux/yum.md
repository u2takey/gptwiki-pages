# yum 
## chatgpt 
yum (Yellowdog Updater Modified) is a package manager for Linux operating systems that automates the installation and update of software packages. It is a command-line tool that searches for, installs, and manages software on the system. 

Here are some basic commands of YUM:

1. yum install packagename - This command installs a specified package and its dependencies.

2. yum update - This command updates all installed packages to their latest versions.

3. yum remove packagename - This command removes a specified package from the system.

4. yum search keyword - This command searches for a package that matches a specified keyword.

5. yum repolist - This command lists all available repositories from where packages can be installed.

6. yum clean all - This command removes all cached packages and metadata from the system.

In summary, YUM is an important package management tool that helps system administrators manage and maintain Linux systems efficiently. 

## tldr 
 
> Package management utility for RHEL, Fedora, and CentOS (for older versions).
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://manned.org/yum>.

- Install a new package:

`yum install {{package}}`

- Install a new package and assume yes to all questions (also works with update, great for automated updates):

`yum -y install {{package}}`

- Find the package that provides a particular command:

`yum provides {{command}}`

- Remove a package:

`yum remove {{package}}`

- Display available updates for installed packages:

`yum check-update`

- Upgrade installed packages to the newest available versions:

`yum upgrade`
