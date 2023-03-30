# pipenv 
## chatgpt 
The `pipenv` command is a tool used to create and manage virtual environments for Python projects. It combines the functionality of two other popular Python tools, `pip` and `virtualenv`, into a single tool. 

When you run the `pipenv` command, it first checks for the `Pipfile` in the current directory. The `Pipfile` file is a configuration file that lists the dependencies of your project which are managed by `pipenv`. If the `Pipfile` file is not found in the current directory, `pipenv` will create a new one for you.

`pipenv` then creates a new virtual environment for your project. A virtual environment is an isolated environment where all the packages and dependencies related to the project are installed. It ensures that the packages installed for one project do not conflict with those installed for another project. 

Once the virtual environment is created, `pipenv` reads the `Pipfile` file and installs the packages listed as dependencies in the virtual environment.

You can also use `pipenv` to install a new package for your project. When you run `pipenv install <package_name>`, `pipenv` checks if the package is already listed in the `Pipfile.lock`. If it is not listed, it installs the package and adds it to the `Pipfile.lock` file.

In summary, the `pipenv` command is used to create and manage virtual environments, track the dependencies of your project, and install/manage packages for your project. 

## tldr 
 
> Simple and unified Python development workflow.
> Manages packages and the virtual environment for a project.
> More information: <https://pypi.org/project/pipenv>.

- Create a new project:

`pipenv`

- Create a new project using Python 3:

`pipenv --three`

- Install a package:

`pipenv install {{package_name}}`

- Install all the dependencies for a project:

`pipenv install`

- Install all the dependencies for a project (including dev packages):

`pipenv install --dev`

- Uninstall a package:

`pipenv uninstall {{package_name}}`

- Start a shell within the created virtual environment:

`pipenv shell`

- Generate a `requirements.txt` (list of dependencies) for a project:

`pipenv lock --requirements`
