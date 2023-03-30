# debuild 
## chatgpt 
The "debuild" command is used in the Debian packaging system to build a Debian package from the source code of a software package. 

When you run the "debuild" command, it performs the following actions:

1. It checks the source code for any errors or packaging issues.
2. It creates a new source package that includes any necessary files, such as the Debian control files, which describe how the package should be installed.
3. It compiles the source code and creates a binary package.
4. It signs the package with your GPG key to ensure that it has not been tampered with.
5. It places the resulting packages in a folder called "debs" in the parent directory.

Overall, the "debuild" command is an essential tool for developers who want to create and distribute their software as a Debian package. It simplifies the packaging process, which can be complex and time-consuming, and ensures that the package is of high quality and will work on a Debian-based system. 

## tldr 
 
> Tool to build a Debian package from source.
> More information: <https://manpages.debian.org/debuild>.

- Build the package in the current directory:

`debuild`

- Build a binary package only:

`debuild -b`

- Do not run lintian after building the package:

`debuild --no-lintian`
