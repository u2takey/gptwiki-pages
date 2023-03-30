# virtualenvwrapper 
## chatgpt 
`virtualenvwrapper` is a Python package that is used as a tool for creating and managing virtual environments in Python. It provides a set of command-line tools which make it easier to access, manage and organize multiple virtual environments, and to maintain the packages installed in them.

Here are some of the most commonly used commands in `virtualenvwrapper`:

- `mkvirtualenv`: This creates a new virtual environment with the specified name.

- `workon`: This lists all available virtual environments and lets the user switch to a specific one. 

- `deactivate`: This exits the current virtual environment, and the user goes back to the global Python environment.

- `rmvirtualenv`: This deletes an existing virtual environment.

- `lssitepackages`: This lists all packages installed globally, but also lists only packages installed locally in the current virtual environment.

- `setvirtualenvproject`: This links the virtual environment to a project directory. When the virtual environment is activated, the associated project directory becomes the current working directory.

`virtualenvwrapper` provides an easy and efficient way to manage multiple Python environments with their unique dependencies, without causing conflicts or interference between them. 

## tldr 
 
> Group of simple wrapper commands for Python's `virtualenv` tool.
> More information: <http://virtualenvwrapper.readthedocs.org>.

- Create a new Python `virtualenv` in `$WORKON_HOME`:

`mkvirtualenv {{virtualenv_name}}`

- Create a `virtualenv` for a specific Python version:

`mkvirtualenv --python {{/usr/local/bin/python3.8}} {{virtualenv_name}}`

- Activate or use a different `virtualenv`:

`workon {{virtualenv_name}}`

- Stop the `virtualenv`:

`deactivate`

- List all virtual environments:

`lsvirtualenv`

- Remove a `virtualenv`:

`rmvirtualenv {{virtualenv_name}}`

- Get summary of all virtualenvwrapper commands:

`virtualenvwrapper`
