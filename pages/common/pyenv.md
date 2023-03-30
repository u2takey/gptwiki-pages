# pyenv 
## chatgpt 
pyenv is a command-line tool used for managing multiple Python versions. It allows developers to easily switch between different versions of Python on their local machine.

When used in the terminal, the pyenv command displays a list of available actions that can be performed, such as:

- `pyenv versions`: Lists all installed Python versions
- `pyenv install`: Installs a specific version of Python
- `pyenv uninstall`: Uninstalls a specific version of Python
- `pyenv global`: Sets the global Python version to be used by the system
- `pyenv local`: Sets the local Python version to be used in a particular directory
- `pyenv shell`: Sets the Python version to be used in the current terminal session

Overall, pyenv is a powerful tool that helps developers manage their Python environment with ease. 

## tldr 
 
> Switch between multiple versions of Python easily.
> More information: <https://github.com/pyenv/pyenv>.

- List all available commands:

`pyenv commands`

- List all Python versions under the `${PYENV_ROOT}/versions` directory:

`pyenv versions`

- List all Python versions that can be installed from upstream:

`pyenv install --list`

- Install a Python version under the `${PYENV_ROOT}/versions` directory:

`pyenv install {{2.7.10}}`

- Uninstall a Python version under the `${PYENV_ROOT}/versions` directory:

`pyenv uninstall {{2.7.10}}`

- Set Python version to be used globally in the current machine:

`pyenv global {{2.7.10}}`

- Set Python version to be used in the current directory and all directories below it:

`pyenv local {{2.7.10}}`
