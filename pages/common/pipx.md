# pipx 
## chatgpt 
pipx is a Python package manager that provides a way to install Python packages as isolated executables. It does this by creating isolated virtual environments for each package, which allows you to install and run different versions of the same package without any conflicts.

The pipx command is used to install and manage Python packages as isolated executables. Here are some of the most commonly used pipx commands:

1. list: This command lists all the packages installed by pipx.
2. install: This command is used to install a package using pipx. The package will be installed as an isolated executable.
3. uninstall: This command is used to uninstall a package that was installed using pipx.
4. upgrade: This command is used to upgrade a package to the latest version.
5. run: This command is used to run an installed package. This allows you to run Python scripts without activating a virtual environment.

Overall, pipx is a useful tool for managing Python packages and creating isolated environments for each package, which helps ensure that there are no conflicts between different versions of packages. 

## tldr 
 
> Install and run python applications in isolated environments.
> More information: <https://github.com/pypa/pipx>.

- Run an app in a temporary virtual environment:

`pipx run {{pycowsay}} {{moo}}`

- Install a package in a virtual environment and add entry points to path:

`pipx install {{package}}`

- List installed packages:

`pipx list`

- Run an app in a temporary virtual environment with a package name different from the executable:

`pipx run --spec {{httpx-cli}} {{httpx}} {{http://www.github.com}}`

- Inject dependencies into an existing virtual environment:

`pipx inject {{package}} {{dependency1 dependency2 ...}}`

- Install a package in a virtual environment with pip arguments:

`pipx install --pip-args='{{pip-args}}' {{package}}`
