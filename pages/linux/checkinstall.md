# checkinstall 
## chatgpt 
The "checkinstall" command is used in Linux-based operating systems to create and install a custom package from source code. It is often used when installing software that is not available in the pre-built package format of the distribution.

When using the "checkinstall" command, instead of simply running the standard installation command (usually "./configure", "make", and "sudo make install"), the command is replaced with "sudo checkinstall". This creates a package (.deb for Debian-based systems or .rpm for Redhat-based systems) containing the files and metadata necessary for the system's package manager to install and manage the software.

The benefit of using "checkinstall" is that it allows for easy installation, upgrade, removal, and system-wide management of custom software. Additionally, it often records information about the software installation process, such as configuration files and installed dependencies, to facilitate future maintenance and upgrades.

Overall, the "checkinstall" command is a powerful tool for Linux system administrators and developers, allowing for easy management of custom software installations and simplifying system maintenance. 

## tldr 
 
> Track the local installation of a software package, and produce a binary package which can be used with a system's native package manager.
> More information: <http://checkinstall.izto.org>.

- Create and install a package with default settings:

`sudo checkinstall --default`

- Create a package but don't install it:

`sudo checkinstall --install={{no}}`

- Create a package without documentation:

`sudo checkinstall --nodoc`

- Create a package and set the name:

`sudo checkinstall --pkgname {{package}}`

- Create a package and specify where to save it:

`sudo checkinstall --pakdir {{path/to/directory}}`
