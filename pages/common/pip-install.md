# pip install 
## chatgpt 
"pip install" is a command used in command-line interface (CLI) to install a Python package from the Python Package Index (PyPI) repository. Here is a detailed explanation of the command:

- "pip" stands for "Pip Installs Packages" and is a package manager for Python used to install, uninstall, and manage Python packages. It is commonly used on Unix-based systems, including macOS and Linux, but it can also be used on Windows.
- "install" is a subcommand in pip that specifies the action to be performed, which is the installation of a Python package.
- The package name comes after the "install" subcommand. It can be the exact name of the package, or it can include the version number or package index URL with the package name.
- Once the command is executed, pip will download and install the specified package and its dependencies on your computer. It will also add the package to the Python environment's list of installed packages, making it available for import in your code.

Examples:
- To install the latest version of the package named "numpy", you can run the command "pip install numpy".
- To install a specific version of the package, you can add the version number after the package name, such as "pip install numpy==1.18.5".
- You can also install packages from other sources using the package index URL. For example, "pip install https://example.com/package.tar.gz". 

## tldr 
 
> Install Python packages.
> More information: <https://pip.pypa.io>.

- Install a package:

`pip install {{package_name}}`

- Install a specific version of a package:

`pip install {{package_name}}=={{package_version}}`

- Install packages listed in a file:

`pip install --requirement {{path/to/requirements.txt}}`

- Install packages from an URL or local file archive (.tar.gz | .whl):

`pip install --find-links {{url|path/to/file}}`

- Install the local package in the current directory in develop (editable) mode:

`pip install --editable {{.}}`
