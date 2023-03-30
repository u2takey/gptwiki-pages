# debootstrap 
## chatgpt 
debootstrap is a command-line tool for bootstrapping a basic Debian or Ubuntu system. It is used to create an initial installation of the operating system on a new or existing system, or to create a minimal chroot environment.

The debootstrap command requires two arguments:
1. The first argument is the name of the distribution to bootstrap.
2. The second argument is the directory where the bootstrap system will be installed

For example, to install a Debian operating system in a directory named "debian_root", the command would look like this: 
```
debootstrap stretch debian_root http://ftp.debian.org/debian
```
This would download and install the Debian stretch distribution in the "debian_root" directory, using the http://ftp.debian.org/debian repository as a source of packages.

debootstrap can also be used with various options to specify additional settings, such as the architectures to include, the type of installation to perform (minimal, standard or full), the proxy server to use, the list of packages to install, and more.

Overall, debootstrap is a powerful tool for administrators who need to quickly set up a basic Debian or Ubuntu system, or to create a minimal environment for testing or development purposes. 

## tldr 
 
> Create a basic Debian system.
> More information: <https://wiki.debian.org/Debootstrap>.

- Create a Debian stable release system inside the `debian-root` directory:

`sudo debootstrap stable {{path/to/debian-root/}} http://deb.debian.org/debian`

- Create a minimal system including only required packages:

`sudo debootstrap --variant=minbase stable {{path/to/debian-root/}}`

- Create an Ubuntu 20.04 system inside the `focal-root` directory with a local mirror:

`sudo debootstrap focal {{path/to/focal-root/}} {{file:///path/to/mirror/}}`

- Switch to a bootstrapped system:

`sudo chroot {{path/to/root}}`

- List available releases:

`ls /usr/share/debootstrap/scripts/`
