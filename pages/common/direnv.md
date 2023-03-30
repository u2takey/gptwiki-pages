# direnv 
## chatgpt 
`direnv` is a command-line tool that allows you to load environment variables, aliases, and other settings automatically when you change directories. 

When you run `direnv`, it will look for a `.envrc` file in the current directory or any of its parent directories. This file contains a set of environment variables and other commands to be executed whenever you navigate to this directory using `cd`.

For example, let's say you have a project that requires you to set an environment variable named `DATABASE_URL`. Instead of manually setting this variable every time you enter the project directory, you can create a `.envrc` file in the directory with the following contents:

```
export DATABASE_URL=postgres://localhost/mydb
```

Now, whenever you `cd` into the project directory, `direnv` will automatically set the `DATABASE_URL` variable for you. Similarly, if you navigate out of the directory, `direnv` will unset the variable so that it doesn't interfere with other projects.

In addition to environment variables, you can also use `direnv` to define aliases, run custom shell commands, and more. This makes it a powerful tool for managing your development environment and automating repetitive tasks. 

## tldr 
 
> Shell extension to load and unload environment variables depending on the current directory.
> More information: <https://github.com/direnv/direnv>.

- Grant direnv permission to load the `.envrc` present in the current directory:

`direnv allow {{.}}`

- Revoke the authorization to load the `.envrc` present in the current directory:

`direnv deny {{.}}`

- Edit the `.envrc` file in the default text editor and reload the environment on exit:

`direnv edit {{.}}`

- Trigger a reload of the environment:

`direnv reload`

- Print some debug status information:

`direnv status`
