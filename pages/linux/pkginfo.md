# pkginfo 
## chatgpt 
The command "pkginfo" is a command that is available in certain Unix and Unix-like operating systems, such as Solaris, AIX, and HP-UX. This command is generally used to display information about software packages that are installed on the system. 

When the command "pkginfo" is executed, it lists all of the software packages that are currently installed on the system with detailed information about each package, including the package name, version number, description, and installation date. This information can be useful for system administrators to manage installed packages and troubleshoot any issues that may arise.

The "pkginfo" command can be used with various options to filter the output, sort the information, or display only specific information about a package. For example, the "-l" option can be used to display more detailed information about each package, while the "-i" option can display only the installation status of a package.

Overall, the "pkginfo" command is a useful tool for managing software packages on a Unix or Unix-like system, providing system administrators with valuable information about software installations and configurations. 

## tldr 
 
> Query the package database on a CRUX system.
> More information: <https://crux.nu/Main/Handbook3-6#ntoc19>.

- List installed packages and their versions:

`pkginfo -i`

- List files owned by a package:

`pkginfo -l {{package_name}}`

- List the owner(s) of files matching a pattern:

`pkginfo -o {{pattern}}`

- Print the footprint of a file:

`pkginfo -f {{path/to/file}}`
