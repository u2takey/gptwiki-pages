# prettier 
## chatgpt 
"Prettier" is a command that refers to a package that is used for code formatting in software development. It helps developers ensure consistency in code styling by automatically formatting code according to a set of rules and guidelines.

The Prettier command can be implemented in different ways depending on the programming language and development environment being used. For example, in JavaScript, the Prettier package can be installed using a package manager such as npm, and then integrated with a code editor or build system.

Once installed, the Prettier command can be used to format code files in a specific directory, a single file, or even as part of a code pipeline or build process. This can be done using various command line options and flags, and can be automated to run automatically whenever code changes are made.

Overall, the Prettier command is a valuable tool for developers looking to improve code quality and maintainability by enforcing consistent code formatting practices. 

## tldr 
 
> An opinionated code formatter for JavaScript, JSON, CSS, YAML, and more.
> More information: <https://prettier.io/>.

- Format a file and print the result to `stdout`:

`prettier {{path/to/file}}`

- Check if a specific file has been formatted:

`prettier --check {{path/to/file}}`

- Run with a specific configuration file:

`prettier --config {{path/to/config_file}} {{path/to/file}}`

- Format a file or directory, replacing the original:

`prettier --write {{path/to/file_or_directory}}`

- Format files or directories recursively using single quotes and no trailing commas:

`prettier --single-quote --trailing-comma {{none}} --write {{path/to/file_or_directory}}`

- Format JavaScript and TypeScript files recursively, replacing the original:

`prettier --write "**/*.{js,jsx,ts,tsx}"`
