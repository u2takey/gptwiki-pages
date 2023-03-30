# dpkg-query 
## chatgpt 
dpkg-query is a command line tool used to query the Debian package database. It is used to display information about the installed packages on a Debian or Ubuntu operating system.

The syntax of the dpkg-query command is as follows:

```
dpkg-query [options] [package_name]
```

Here, `[options]` are the various options available with the command and `[package_name]` is the name of the package for which we need information.

Some commonly used options with the dpkg-query command are as follows:

- `-l`: This option lists all installed packages on the system.
- `-s`: This option displays the status of the package.
- `-p`: This option displays detailed information about the package.
- `-W`: This option shows the name of the installed package.
- `--showformat`: This option specifies the format of the output.

For example, the command `dpkg-query -l` will list all the installed packages on the system along with their version numbers, descriptions, and other details.

Similarly, the command `dpkg-query -s firefox` will show the status of the Firefox package installed on the system.

The `dpkg-query` command is a powerful tool that can be used to perform various package management tasks on a Debian or Ubuntu system. 

## tldr 
 
> A tool that shows information about installed packages.
> More information: <https://manpages.debian.org/latest/dpkg/dpkg-query.1.html>.

- List all installed packages:

`dpkg-query --list`

- List installed packages matching a pattern:

`dpkg-query --list '{{libc6*}}'`

- List all files installed by a package:

`dpkg-query --listfiles {{libc6}}`

- Show information about a package:

`dpkg-query --status {{libc6}}`

- Search for packages that own files matching a pattern:

`dpkg-query --search {{/etc/ld.so.conf.d}}`
