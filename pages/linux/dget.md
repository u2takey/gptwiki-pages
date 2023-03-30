# dget 
## chatgpt 
dget is a Debian-specific command that is used to download and apply source packages from the Debian archive. It downloads the .dsc, .tar.gz, and .diff.gz files of the specified source package and extracts the source files contained within.

The command would typically be used by a Debian package maintainer who needs to update an existing Debian package. It allows the maintainer to download the latest version of the source package (along with any associated patches) from the Debian archive, make any needed changes, and then rebuild the package.

Here's the syntax for the dget command:

dget [options] <dsc-url>

The <dsc-url> parameter should be the URL to the .dsc file for the package you want to download. The options that can be used with the dget command include:

- -d: Download only the .dsc file and not the associated source files
- -u: Unpack the source package but do not apply any patches
- -x: Extract the source package and apply any patches

Overall, the dget command is a useful tool for Debian package maintainers who need to work with source packages from the Debian archive. 

## tldr 
 
> Download Debian packages.
> More information: <https://manpages.debian.org/dget>.

- Download a binary package:

`dget {{package_name}}`

- Download and extract a package source from its `.dsc` file:

`dget {{http://deb.debian.org/debian/pool/main/h/haskell-tldr/haskell-tldr_0.4.0-2.dsc}}`

- Download a package source tarball from its `.dsc` file but don't extract it:

`dget -d {{http://deb.debian.org/debian/pool/main/h/haskell-tldr/haskell-tldr_0.4.0-2.dsc}}`
