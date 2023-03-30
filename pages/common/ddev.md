# ddev 
## chatgpt 
ddev is a command-line tool used for local web development. It is used to manage local development environments for PHP-based web applications on Linux, Mac, and Windows operating systems. 

Here are some of the commands you can use with `ddev`:

- `ddev config`: This command is used to view and edit the configuration file for the ddev project.
- `ddev start`: This command is used to start a ddev project.
- `ddev stop`: This command is used to stop a ddev project.
- `ddev restart`: This command is used to restart a ddev project.
- `ddev ssh`: This command is used to open an SSH connection to the server running the ddev project.
- `ddev exec`: This command is used to execute a command in the context of the ddev project.
- `ddev list`: This command is used to list all of the ddev projects currently available.

Overall, ddev is a powerful tool for web developers looking to create and manage local development environments for their PHP-based web applications. 

## tldr 
 
> Container based local development tool for PHP environments.
> More information: <https://ddev.readthedocs.io>.

- Start up a project:

`ddev start`

- Configure a project's type and docroot:

`ddev config`

- [f]ollow the log trail:

`ddev logs -f`

- Run composer within the container:

`ddev composer`

- Install a specific Node.js version:

`ddev nvm install {{version}}`

- Export a database:

`ddev export-db --file={{/tmp/db.sql.gz}}`

- Run a specific command within a container:

`ddev exec {{echo 1}}`
