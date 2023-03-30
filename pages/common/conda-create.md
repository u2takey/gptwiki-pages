# conda create 
## chatgpt 
`conda create` is a command used in the terminal or command prompt to create a new Python environment using the Conda package manager. 

Here's how the command works in detail:

1. Open the terminal or command prompt
2. Type `conda create` followed by various options and arguments
3. Hit Enter to execute the command

The basic syntax for the `conda create` command is:

```
conda create --name env_name package_name
```

- `env_name`: The name of the new environment you want to create. This is a required argument.
- `package_name`: The name of the package that you want to install in the new environment. This is an optional argument, but recommended to specify to avoid conflicts with other packages.

Other common options and arguments you can include with the `conda create` command include:

- `--clone existing_env`: Creates a new environment by cloning an existing one.
- `-p path/to/env`: Creates an environment in a specific directory, rather than the default location.
- `-y`: Skips the confirmation prompt.

Once you run the `conda create` command, Conda will create a new environment with the specified name and optionally install the specified package(s). You can activate the new environment using the `conda activate env_name` command, and deactivate it using `conda deactivate`. 

## tldr 
 
> Create new conda environments.
> More information: <https://docs.conda.io/projects/conda/en/latest/commands/create.html>.

- Create a new environment named `py39`, and install Python 3.9 and NumPy v1.11 or above in it:

`conda create --yes --name {{py39}} python={{3.9}} "{{numpy>=1.11}}"`

- Make exact copy of an environment:

`conda create --clone {{py39}} --name {{py39-copy}}`

- Create a new environment with a specified name and install a given package:

`conda create --name {{env_name}} {{package_name}}`
