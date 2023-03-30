# pip 
## chatgpt 
Pip is a command-line tool that allows you to install, manage, and work with Python packages. It is commonly used in Python development to install packages that are not included in the standard library. 

Here are some of the most common commands associated with pip:

1. pip install <package_name>: This command is used to install the specified package. For example, “pip install numpy” will install the popular numpy library.

2. pip uninstall <package_name>: This command is used to uninstall the specified package.

3. pip list: This command is used to list all the packages installed in the current environment.

4. pip freeze: This command is used to list all the packages and their version numbers installed in the current environment. This is often used to generate a requirements.txt file that can be used to recreate the environment on another machine.

5. pip show <package_name>: This command is used to display detailed information about the specified package, including its version, dependencies, and installation location. 

6. pip search <query>: This command is used to search the python package index (PyPI) for packages that match the specified query.

7. pip install --upgrade <package_name>: This command is used to upgrade the specified package to the latest version if available.

These are just a few of the many commands available with pip. Overall, pip is an essential tool for anyone working with Python packages, and is included by default with most versions of Python. 

## tldr 
 
> Python package manager.
> Some subcommands such as `pip install` have their own usage documentation.
> More information: <https://pip.pypa.io>.

- Install a package (see `pip install` for more install examples):

`pip install {{package_name}}`

- Install a package to the user's directory instead of the system-wide default location:

`pip install --user {{package}}`

- Upgrade a package:

`pip install --upgrade {{package_name}}`

- Uninstall a package:

`pip uninstall {{package_name}}`

- Save installed packages to file:

`pip freeze > {{requirements.txt}}`

- Show installed package info:

`pip show {{package_name}}`

- Install packages from a file:

`pip install --requirement {{requirements.txt}}`
