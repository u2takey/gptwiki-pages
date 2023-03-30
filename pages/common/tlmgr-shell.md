# tlmgr shell 
## chatgpt 
`tlmgr` is the TeX Live package manager command-line tool used to install, manage, and update packages in a TeX Live distribution. 

The `tlmgr shell` command opens up a new command shell with a restricted environment, where the only available command is `tlmgr`, and all other system commands are disabled. This prevents conflicts between packages installed with `tlmgr` and packages installed through other means, such as a Linux package manager. 

Opening a new shell with a restricted environment ensures that the `tlmgr` command will work as intended without interference from external factors. With this shell, users can work seamlessly within the package management system of TeX Live. 

## tldr 
 
> Start an interactive shell of the native TeX Live manager.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Start an interactive shell of `tlmgr`:

`tlmgr shell`

- Run any `tlmgr` sub-command in the interactive shell:

`{{sub_command}} {{arguments}}`

- Quit the interactive shell:

`quit`

- List all TeX Live variables:

`get`

- Get the value of a TeX Live variable:

`get {{variable}}`

- Set the value of a TeX Live variable:

`set {{variable}} {{value}}`

- Restart the interactive shell:

`restart`

- Print the version of the current protocol:

`protocol`
