# makepkg 
## chatgpt 
The `makepkg` command is a utility program in Linux operating systems that assists in creating custom packages from source code. This command is specifically used in Arch Linux and its derivatives.

When running the `makepkg` command, it will search for a `PKGBUILD` file in the current directory. The `PKGBUILD` file contains a set of instructions that specify how the package is built and installed. 

Once the `PKGBUILD` file is found, `makepkg` will create a package using the instructions contained in the file. This process may involve downloading and compiling the source code, copying the necessary files into a package directory, creating a package metadata file, and compressing the entire package.

The resulting package can then be installed using the package manager (e.g., pacman) of the Linux system where it is intended to be used. 

Overall, the `makepkg` command is a useful tool for creating custom packages in Arch Linux, as it automates the process of building, installing, and managing packages. 

## tldr 
 
> Create a package which can be used with `pacman`.
> Uses the `PKGBUILD` file in the current working directory by default.
> More information: <https://man.archlinux.org/man/makepkg.8>.

- Make a package:

`makepkg`

- Make a package and install its dependencies:

`makepkg --syncdeps`

- Make a package, install its dependencies then install it to the system:

`makepkg --syncdeps --install`

- Make a package, but skip checking the source's hashes:

`makepkg --skipchecksums`

- Clean up work directories after a successful build:

`makepkg --clean`

- Verify the hashes of the sources:

`makepkg --verifysource`

- Generate and save the source information into `.SRCINFO`:

`makepkg --printsrcinfo > .SRCINFO`
