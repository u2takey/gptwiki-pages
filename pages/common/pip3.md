# pip3 
## chatgpt 
pip3 is a command line tool for installing Python packages. 

"Pip" stands for "Pip Installs Packages." It is the package installer for Python. Pip is an essential tool as it simplifies the task of installing and managing Python packages/modules/libraries of different versions. Pip is the preferred installer program.

The "3" in "pip3" refers to the Python version. There are two main versions of Python: Python 2.x and Python 3.x. The pip3 command is used when working with Python 3.x, while pip is used for Python 2.x.

When you type "pip3" in the terminal or command prompt, you can use various subcommands after it to perform different actions, such as installing, upgrading, and removing packages. 

Here are some examples of how to use pip3:

- To install a package: pip3 install package_name
- To upgrade a package: pip3 install --upgrade package_name
- To remove a package: pip3 uninstall package_name
- To list all installed packages: pip3 list
- To show package information: pip3 show package_name

Overall, pip3 is a powerful command line tool that simplifies the process of working with Python packages. 

## tldr 
 
> Python package manager.
> More information: <https://pip.pypa.io>.

- Find available packages:

`pip3 search {{package_name}}`

- Install a package:

`pip3 install {{package_name}}`

- Install a specific version of a package:

`pip3 install {{package_name}}=={{package_version}}`

- Upgrade a package:

`pip3 install --upgrade {{package_name}}`

- Uninstall a package:

`pip3 uninstall {{package_name}}`

- Save the list of installed packages to a file:

`pip3 freeze > {{requirements.txt}}`

- Install packages from a file:

`pip3 install --requirement {{requirements.txt}}`

- Show installed package info:

`pip3 show {{package_name}}`
