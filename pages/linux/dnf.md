# dnf 
## chatgpt 
DNF (short for Dandified YUM) is a command-line package manager used in most Linux distributions based on Fedora, including Fedora, Red Hat Enterprise Linux, and CentOS. DNF is the successor to the YUM package manager and offers several improvements like faster operation and dependency resolution, multiple interface support, and better security handling.

Using DNF, users can install, update, remove, and manage software packages on their system. Below are some example commands:

- Install a package: `dnf install packagename`

- Update packages: `dnf update`

- Remove a package: `dnf remove packagename`

- Search for a package: `dnf search packagename`

- Display information about a package: `dnf info packagename`

- List all installed packages: `dnf list installed`

- Check for package dependencies: `dnf repoquery --requires packagename`

- List all available repositories: `dnf repolist`

It's worth noting that DNF requires root or superuser privileges to run most of the commands. As such, you'll typically need to use the `sudo` command or log in as the root user to use DNF effectively. 

## tldr 
 
> Package management utility for RHEL, Fedora, and CentOS (replaces yum).
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://dnf.readthedocs.io>.

- Upgrade installed packages to the newest available versions:

`sudo dnf upgrade`

- Search packages via keywords:

`dnf search {{keywords}}`

- Display details about a package:

`dnf info {{package}}`

- Install a new package (use `-y` to confirm all prompts automatically):

`sudo dnf install {{package}}`

- Remove a package:

`sudo dnf remove {{package}}`

- List installed packages:

`dnf list --installed`

- Find which packages provide a given file:

`dnf provides {{file}}`

- View all past operations:

`dnf history`
