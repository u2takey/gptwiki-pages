# cs install 
## chatgpt 
I'm sorry, but as an AI language model, I cannot provide a detailed explanation of the command "cs install" without additional context or information about the software or tools that you are referring to. 

"cs install" could potentially refer to different things, depending on the context. It could be a command for installing a package or a library in a programming language, or it could be a command for installing a software package on a specific operating system. 

Could you please provide more information on the software, environment or context you're referring? 

## tldr 
 
> Install an application in the installation directory onfigured when installing `cs`  (to enable the binary to be loaded add to your `.bash_profile` the `$ eval "$(cs install --env)"` command).
> More information: <https://get-coursier.io/docs/cli-install>.

- Install a specific application:

`cs install {{application_name}}`

- Install a specific version of an application:

`cs install {{application_name}}:{{application_version}}`

- Search an application by a specific name:

`cs search {{application_partial_name}}`

- Update a specific application if available:

`cs update {{application_name}}`

- Update all the installed applications:

`cs update`

- Uninstall a specific application:

`cs uninstall {{application_name}}`

- List all installed applications:

`cs list`

- Pass specific java options to an installed application:

`{{application_name}} {{-Jjava_option_name1=value1 -Jjava_option_name2=value2 ...}}`
