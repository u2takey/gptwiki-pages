# dkms 
## chatgpt 
DKMS (Dynamic Kernel Module Support) is a framework that allows the creation of Linux kernel modules that can be automatically rebuilt when a new kernel version is installed. The dkms command is used to manage these kernel modules.

The syntax of the command is:

```
dkms [options] <command>
```

The options can be used to specify the DKMS configuration file, set the verbosity level, or control whether the command should be executed with superuser (root) privileges.

The available commands are:

- add: adds a new module to DKMS
- build: builds or rebuilds the module for the current kernel version
- install: installs the module for the current kernel version
- remove: removes the module from DKMS
- uninstall: removes the module from the current kernel version
- status: shows the status of all installed modules and their versions
- mktarball: creates a tarball for manual installation of the module
- mkdeb: creates a Debian package for installation of the module
- mkpkg: creates a package for installation of the module on non-Debian systems
- autoinstall: builds and install the module for all available kernel versions
- mkkpkg: creates a kernel package for easy installation of the module on other systems

Overall, dkms is an extremely useful tool for managing kernel modules, particularly for system administrators and developers who need to update and maintain kernel modules across multiple systems. 

## tldr 
 
> A framework that allows for dynamic building of kernel modules.
> More information: <https://github.com/dell/dkms>.

- List currently installed modules:

`dkms status`

- Rebuild all modules for the currently running kernel:

`dkms autoinstall`

- Install version 1.2.1 of the acpi_call module for the currently running kernel:

`dkms install -m {{acpi_call}} -v {{1.2.1}}`

- Remove version 1.2.1 of the acpi_call module from all kernels:

`dkms remove -m {{acpi_call}} -v {{1.2.1}} --all`
