# rpm 
## chatgpt 
The rpm command is a useful package management tool in Linux-based operating systems. It stands for "RPM Package Manager" and is used to install, update, query or remove software packages in the system. 

The syntax of rpm command is as follows:

rpm [options] [package]

Some of the commonly used options and their meanings are:

-c: Check the package file(s) for errors
-d: Print out the dependencies of the specified package
-e: Erase/remove the installed package from the system
-i: Install a package in the system
-q: Query the package database
-u: Upgrade an existing package

Additionally, some other important options are:

-h: Display help information about rpm command
-v: Enable verbose output for rpm command
-a: Query all packages in the system
-f: Query which package owns a specific file
--nodeps: Install a package without checking for dependencies

Overall, rpm command provides a powerful set of functionalities for managing software packages in Linux-based operating systems. With its various command options, you can easily install or remove software, check for package dependencies, and query the package database to find out information about installed packages. 

## tldr 
 
> RPM Package Manager.
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://rpm.org/>.

- Show version of httpd package:

`rpm --query {{httpd}}`

- List versions of all matching packages:

`rpm --query --all '{{mariadb*}}'`

- Forcibly install a package regardless of currently installed versions:

`rpm --upgrade {{package_name.rpm}} --force`

- Identify owner of a file and show version of the package:

`rpm --query --file {{/etc/postfix/main.cf}}`

- List package-owned files:

`rpm --query --list {{kernel}}`

- Show scriptlets from an RPM file:

`rpm --query --package --scripts {{package_name.rpm}}`

- Show changed, missing and/or incorrectly installed files of matching packages:

`rpm --verify --all '{{php-*}}'`

- Display the changelog of a specific package:

`rpm --query --changelog {{package_name}}`
