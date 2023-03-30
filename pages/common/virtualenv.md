# virtualenv 
## chatgpt 
The "virtualenv" command is used to create isolated Python environments. 

When you install packages and dependencies for a particular project, it's recommended to install them in an isolated virtual environment rather than globally. This helps in avoiding conflicts between packages installed in different projects.

To create a virtual environment using the "virtualenv" command, you need to provide a name for the environment and a path in which to create it. Here's an example:

```
virtualenv my_env
```

This will create a virtual environment called "my_env" in the current directory.

You can also specify the Python interpreter for the virtual environment using the "--python" option. For example:

```
virtualenv --python=python3 my_env
```

This will create a virtual environment using the Python 3 interpreter.

Once the virtual environment is created, you can activate it using the following command:

```
source my_env/bin/activate
```

This will activate the virtual environment and any packages you install while it's active will be installed only in this environment.

To deactivate the virtual environment, simply use the "deactivate" command:

```
deactivate
```

This will return you to the system's default Python environment. 

## tldr 
 
> Create virtual isolated Python environments.
> More information: <https://virtualenv.pypa.io/>.

- Create a new environment:

`virtualenv {{path/to/venv}}`

- Customize the prompt prefix:

`virtualenv --prompt={{prompt_prefix}} {{path/to/venv}}`

- Use a different version of Python with virtualenv:

`virtualenv --python={{path/to/pythonbin}} {{path/to/venv}}`

- Start (select) the environment:

`source {{path/to/venv}}/bin/activate`

- Stop the environment:

`deactivate`
