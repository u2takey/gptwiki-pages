# pkgmk 
## chatgpt 
The pkgmk command is a package building tool in the Solaris and OpenSolaris operating systems. It is used to build software packages from source code so that they can be easily installed and managed on a system.

Here is the detail of the pkgmk command:

Usage: pkgmk [-a adminfile] [-b] [-d destination_directory] [-f pkginfo_file] [-o options_file] [-r root_directory] [-v version] [-x exclude_list_file] [source_directory]

Options:

- [-a adminfile] - Specifies the file that contains the package admin information such as ownership, permissions, and dependencies.
- [-b] - Specifies that the binary package be created instead of the text version.
- [-d destination_directory] - Specifies the directory where the package file will be placed once it is built.
- [-f pkginfo_file] - Specifies the file that contains the package information such as the package name, version, and description.
- [-o options_file] - Specifies the file that contains additional options for the pkgmk command.
- [-r root_directory] - Specifies the root directory where the package software will be installed.
- [-v version] - Specifies the version of the package being created.
- [-x exclude_list_file] - Specifies the file that contains a list of files and directories to exclude from the package.

The source_directory argument specifies the location of the source files that will be used to build the package.

Once the pkgmk command is run with the appropriate options and arguments, it will create a package file that can be installed on a system using the pkgadd command. The package file will automatically handle file installation, removal, and dependencies. This makes it easier to manage software installations and updates on a system. 

## tldr 
 
> Make a binary package for use with pkgadd on CRUX.
> More information: <https://docs.oracle.com/cd/E19683-01/816-0210/6m6nb7mha/index.html>.

- Make and download a package:

`pkgmk -d`

- Install the package after making it:

`pkgmk -d -i`

- Upgrade the package after making it:

`pkgmk -d -u`

- Ignore the footprint when making a package:

`pkgmk -d -if`

- Ignore the MD5 sum when making a package:

`pkgmk -d -im`

- Update the package's footprint:

`pkgmk -uf`
