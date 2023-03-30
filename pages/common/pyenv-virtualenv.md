# pyenv virtualenv 
## chatgpt 
`pyenv virtualenv` is a command used with the Python version manager tool `pyenv` to create a new virtual environment. 

A virtual environment is an isolated environment where different versions of Python and Python packages can be installed without affecting the system's core Python installation. This allows developers to work on multiple projects with different package requirements without conflicts.

The `pyenv virtualenv` command is used to create a new virtual environment with a specified name and a particular version of Python. The general syntax for this command is:

```
pyenv virtualenv <python_version> <environment_name>
```

For example, to create a new virtual environment with Python 3.9.5 and name it "my_project_venv", you would use the following command:

```
pyenv virtualenv 3.9.5 my_project_venv
```

This command will create a new directory under the `~/.pyenv/versions/` directory with the specified name (`my_project_venv`) and Python version (`3.9.5`) for the virtual environment.

Once the virtual environment is created, you can activate it using the `pyenv activate` command:

```
pyenv activate my_project_venv
```

This will activate the virtual environment and allow you to install packages and run Python scripts using the version of Python installed in the virtual environment. 

To deactivate the virtual environment, simply use the `pyenv deactivate` command:

```
pyenv deactivate
```

This will return you to the system's core Python installation. 

## tldr 
 
> Create virtual environments based on one's installed Python distributions.
> More information: <https://github.com/pyenv/pyenv-virtualenv>.

- Create a new Python 3.6.6 virtual environment:

`pyenv virtualenv {{3.6.6}} {{virtualenv_name}}`

- List all existing virtual environments:

`pyenv virtualenvs`

- Activate a virtual environment:

`pyenv activate {{virtualenv_name}}`

- Deactivate the virtual environment:

`pyenv deactivate`
