# wp 
## chatgpt 
The "wp" command is used in the WordPress command-line interface (CLI) to interact with WordPress installations from a terminal or console. It has functions for managing WordPress installations, including managing posts, pages, users, multimedia, plugins, and themes. 

The syntax for the "wp" command is as follows:

    wp <command> [<sub-command>] [--option=value]

The "command" specifies the main function to be executed, such as "post" for managing posts, "user" for managing users, or "plugin" for managing plugins. 

The "sub-command" is optional and specifies a specific action to be taken within the main command. For example, within the "post" command, the sub-commands may include "create", "update", "delete", "list", etc.

The "--option=value" format is used to specify options that modify the behavior of the command. These options may include flags like "--verbose" or "--dry-run", and additional parameters necessary for the command to execute.

Overall, the "wp" command is a powerful tool for managing WordPress installations from the command line, and can greatly improve productivity and efficiency for developers and system administrators. 

## tldr 
 
> The official command-line interface to manage WordPress instances.
> More information: <https://wp-cli.org/>.

- Print information about the operating system, shell, PHP, and WP-CLI (`wp`) installation:

`wp --info`

- Update WP-CLI:

`wp cli update`

- Download a fresh WordPress installation to current directory, optionally specifying the locale:

`wp core download --locale={{locale}}`

- Create basic `wpconfig` file (assuming database on `localhost`):

`wp config create --dbname={{dbname}} --dbuser={{dbuser}} --dbpass={{dbpass}}`

- Install and activate a WordPress plugin:

`wp plugin install {{plugin}} --activate`

- Replace all instances of a string in the database:

`wp search-replace {{old_string}} {{new_string}}`

- Import the contents of a WordPress Extended RSS (WXR) file:

`wp import {{path/to/file.xml}}`
