# conda 
## chatgpt 
The `conda` command is a command-line interface (CLI) tool for managing package dependencies in Python. It is an open-source package management system and environment management system that helps to install, manage, and update packages and their dependencies. 

Here are some of the commonly used options and sub-commands with the `conda` command:

- `conda install`: installs packages that are not already installed, along with their dependencies.
- `conda search`: searches for packages in the available channels.
- `conda update`: updates one or more packages, along with their dependencies.
- `conda remove`: removes one or more packages and their dependencies.
- `conda create`: creates a new environment with the specified packages and their dependencies.
- `conda activate`: activates a specified environment.
- `conda deactivate`: deactivates the active environment.

Overall, `conda` is a powerful tool for managing packages and environments in Python and is widely used by data scientists and developers to efficiently manage their Python projects. 

## tldr 
 
> Package, dependency and environment management for any programming language.
> Some subcommands such as `conda create` have their own usage documentation.
> More information: <https://github.com/conda/conda>.

- Create a new environment, installing named packages into it:

`conda create --name {{environment_name}} {{python=3.9 matplotlib}}`

- List all environments:

`conda info --envs`

- Load an environment:

`conda activate {{environment_name}}`

- Unload an environment:

`conda deactivate`

- Delete an environment (remove all packages):

`conda remove --name {{environment_name}} --all`

- Install packages into the current environment:

`conda install {{python=3.4 numpy}}`

- List currently installed packages in current environment:

`conda list`

- Delete unused packages and caches:

`conda clean --all`
