# dpkg-deb 
## chatgpt 
dpkg-deb is a command-line tool for manipulating Debian (.deb) packages on Linux systems. Here are some of the most common uses:

1. Creating a .deb package from source code: dpkg-deb can create a .deb package from the build output of source code. For example, if you have a folder containing the binary and configuration files for your software, you can use dpkg-deb to turn it into a .deb package that can be installed on other systems.

2. Extracting files from an existing package: dpkg-deb can be used to extract individual files or groups of files from a .deb package. This is useful for examining or modifying the contents of a package.

3. Checking the integrity of a package: dpkg-deb can verify that a .deb package has not been tampered with or corrupted. This is important when handling packages from untrusted sources.

4. Installing or removing a package: dpkg-deb can be used to install or remove a .deb package from the system. This is similar to using the apt-get command, but provides more fine-grained control over the installation process.

Overall, dpkg-deb is a versatile tool for working with Debian packages on Linux systems. It is commonly used by developers, system administrators, and power users who need to work with software packages in a flexible and efficient manner. 

## tldr 
 
> Pack, unpack and provide information about Debian archives.
> More information: <https://manpages.debian.org/latest/dpkg/dpkg-deb.html>.

- Display information about a package:

`dpkg-deb --info {{path/to/file.deb}}`

- Display the package's name and version on one line:

`dpkg-deb --show {{path/to/file.deb}}`

- List the package's contents:

`dpkg-deb --contents {{path/to/file.deb}}`

- Extract package's contents into a directory:

`dpkg-deb --extract {{path/to/file.deb}} {{path/to/directory}}`

- Create a package from a specified directory:

`dpkg-deb --build {{path/to/directory}}`
