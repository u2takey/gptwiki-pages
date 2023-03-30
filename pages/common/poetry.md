# poetry 
## chatgpt 
Poetry is a command-line tool that helps in managing python package dependencies and creating virtual environments. Poetry simplifies the process of installing dependencies and maintaining a virtual environment for your python project. 

Poetry comes with many features like dependency resolution, version management, easy integration with various command-line interfaces, and package distribution. Some of the key features of poetry are:

- Dependency resolution: Poetry manages the dependencies of your project intelligently, making sure that all the packages are compatible with each other. It searches for the latest compatible version and installs it automatically.

- Virtual environment management: Poetry creates a virtual environment for your project that isolates it from the system-wide packages. This ensures that your project dependencies are isolated and won't interfere with other system packages.

- Easy packaging: Poetry provides a simple and intuitive command-line interface to package your project. It creates a distributable package and ensures that all the necessary dependencies are included.

Poetry also supports other features like project scaffolding, Git integration, and more. In summary, Poetry is a powerful tool for managing dependencies and creating virtual environments for your python projects. 

## tldr 
 
> Manage Python packages and dependencies.
> More information: <https://python-poetry.org/docs/cli/>.

- Create a new Poetry project in the directory with a specific name:

`poetry new {{project_name}}`

- Install a dependency and its subdependencies:

`poetry add {{dependency}}`

- Install a development dependency and its subdependencies:

`poetry add --group dev {{dependency}}`

- Interactively initialize the current directory as a new Poetry project:

`poetry init`

- Get the latest version of all dependencies and update `poetry.lock`:

`poetry update`

- Execute a command inside the project's virtual environment:

`poetry run {{command}}`

- Bump the minor version of the project in `pyproject.toml`:

`poetry version minor`
