# toolbox create 
## chatgpt 
The "toolbox create" command is a command-line instruction that creates a new toolbox in MATLAB. A toolbox is a collection of MATLAB functions, scripts, and data files that extend the functionality of MATLAB. 

When executed, this command creates a new toolbox with the specified name in the current directory. It prompts the user with a series of questions to configure the toolbox, such as the author's name, version number, and function prefix. 

After the configuration is complete, MATLAB generates a basic directory structure for the new toolbox, including a "Contents.m" file, which serves as the toolbox's main documentation file. 

The user can then add their own MATLAB functions, scripts, and data files to the toolbox directory to extend the functionality of MATLAB. 

This command is typically used by MATLAB users who wish to create their own custom toolbox to simplify their workflow and enhance their MATLAB programming capabilities. 

## tldr 
 
> Create a new `toolbox` container.
> More information: <https://manned.org/toolbox-create.1>.

- Create a `toolbox` container for a specific distribution:

`toolbox create --distro {{distribution}}`

- Create a `toolbox` container for a specific release of the current distribution:

`toolbox create --release {{release}}`

- Create a `toolbox` container with a custom image:

`toolbox create --image {{name}}`

- Create a `toolbox` container from a custom Fedora image:

`toolbox create --image {{registry.fedoraproject.org/fedora-toolbox:36}}`

- Create a `toolbox` container using the default image for Fedora 36:

`toolbox create --distro {{fedora}} --release {{f36}}`
