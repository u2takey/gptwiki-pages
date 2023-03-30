# mamba 
## chatgpt 
Mamba is a package manager for scientific computing based on Conda. Like Conda, mamba is used to install, update, and manage packages, environments, and channels in a programming language- and operating system-agnostic way.

The mamba command can be used to manage packages and environments by running subcommands, such as "install", "update", "remove", or "create". Some common examples of how to use mamba command are:

- Installing a package: $ mamba install <packagename>
This command will install the specified package (e.g., numpy, pandas, matplotlib) into the current environment or a specific environment specified by the user.

- Updating a package: $ mamba update <packagename>
This command will update the specified package (e.g., numpy, pandas, matplotlib) to the latest version available in the current environment or a specific environment specified by the user.

- Creating a new environment: $ mamba create --name <envname> <packagelist>
This command will create a new environment with the specified name and install the packages listed in <packagelist>.

- Activating an environment: $ mamba activate <envname>
This command will activate the specified environment, allowing the user to run the packages and programs installed in the environment.

Overall, mamba provides an efficient and flexible way to manage software packages for scientific computing, making it easier to install and use the many tools available for data analysis, machine learning, and scientific research. 

## tldr 
 
> Fast, cross-platform package manager, intended as a drop-in replacement for conda.
> Some subcommands such as `mamba repoquery` have their own usage documentation.
> More information: <https://mamba.readthedocs.io/en/latest/user_guide/mamba.html>.

- Create a new environment, installing the specified packages into it:

`mamba create --name {{environment_name}} {{python=3.10 matplotlib}}`

- Install packages into the current environment, specifying the package [c]hannel:

`mamba install -c {{conda-forge}} {{python=3.6 numpy}}`

- Update all packages in the current environment:

`mamba update --all`

- Search for a specific package across repositories:

`mamba repoquery search {{numpy}}`

- List all environments:

`mamba info --envs`

- Remove unused [p]ackages and [t]arballs from the cache:

`mamba clean -pt`

- Activate an environment:

`mamba activate {{environment_name}}`

- List all installed packages in the currently activated environment:

`mamba list`
