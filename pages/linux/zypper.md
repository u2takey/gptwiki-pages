# zypper 
## chatgpt 
zypper is a command-line tool that is used in the openSUSE and SUSE Linux operating systems to manage packages and repositories. It allows users to download and install software packages, update the system, and manage dependencies and conflicts between packages.

The basic syntax for the zypper command is:

zypper [options] [command]

Some of the most commonly used options and commands for zypper include:

- update: updates the system with the latest available packages from the configured repositories.

- install: Installs one or more packages from the configured repositories. For example, "sudo zypper install firefox" installs the Firefox web browser.

- search: searches the configured repositories for packages that match a given keyword or pattern. For example, "sudo zypper search python" lists all packages related to the Python programming language.

- remove: removes one or more packages that are currently installed on the system.

- refresh: updates the information about the available packages in the configured repositories.

- clean: cleans the package cache and removes unneeded packages from the system to free up disk space.

- repo-add: adds a new repository to the list of configured repositories. For example, "sudo zypper repo-add https://download.opensuse.org/repositories/home:myuser/openSUSE_Tumbleweed/home:myuser.repo" adds a new repository provided by a user called "myuser".

Overall, the zypper command is a powerful and flexible tool for managing packages and repositories on a SUSE-based operating system. 

## tldr 
 
> SUSE & openSUSE package management utility.
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://en.opensuse.org/SDB:Zypper_manual>.

- Synchronize list of packages and versions available:

`zypper refresh`

- Install a new package:

`zypper install {{package}}`

- Remove a package:

`zypper remove {{package}}`

- Upgrade installed packages to the newest available versions:

`zypper update`

- Search package via keyword:

`zypper search {{keyword}}`

- Show information related to configured repositories:

`zypper repos --sort-by-priority`
