# install-tl 
## chatgpt 
"install-tl" is a command used to install TeX Live, a comprehensive distribution of the TeX document preparation system. This command is intended for users who want to install TeX Live on their operating system. 

When you type "install-tl" in the command line, it will execute the installation program for TeX Live. The program will ask you to choose installation parameters such as the installation mode (full, minimal, or custom), the installation directory, and the package source. 

The installation mode determines the level of packages that will be installed. The full installation mode installs all the packages available in TeX Live, while the minimal mode installs only a basic set of packages. The custom mode allows you to choose which packages you want to install.

The installation directory specifies the location where TeX Live will be installed on your system. By default, it will be installed in the /usr/local/texlive directory. 

The package source determines the location from which packages will be downloaded during the installation process. The default package source is the CTAN (Comprehensive TeX Archive Network) repository.

Once you have specified the installation parameters, the installation program will begin downloading and installing the selected packages. The process may take some time depending on the size of the packages being installed and your internet connection speed.

Overall, "install-tl" is a command that allows you to easily install TeX Live and begin using the TeX document preparation system on your computer. 

## tldr 
 
> TeX Live cross-platform installer.
> More information: <https://tug.org/texlive/>.

- Start the text-based installer (default on Unix systems):

`install-tl -no-gui`

- Start the GUI installer (default on macOS and Windows, requires Tcl/Tk):

`install-tl -gui`

- Install TeX Live as defined in a specific profile file:

`install-tl -profile {{path/to/texlive.profile}}`

- Start the installer with the settings from a specific profile file:

`install-tl -init-from-file {{path/to/texlive.profile}}`

- Start the installer for installation on a portable device, like a USB stick:

`install-tl -portable`

- Show help for `install-tl`:

`install-tl -help`
