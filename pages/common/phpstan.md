# phpstan 
## chatgpt 
`phpstan` is a command-line tool used for static analysis of PHP code. It helps developers find bugs and errors in their code before it is executed. 

When you run `phpstan` in your terminal, it scans your PHP files and analyzes them for potential bugs and errors. It checks for type mismatches, undefined functions or variables, dead code, and more. 

`phpstan` uses a combination of PHPDoc comments and type inference to analyze the code. It also supports modern PHP features like anonymous classes, generics, and union types. 

The output of `phpstan` includes a list of the issues found in your code, along with the line numbers and descriptions of the problems. This can help you debug and fix issues quickly and easily.

In summary, `phpstan` is a powerful tool that can help developers catch bugs and errors before they cause issues in production. It is particularly useful for large codebases and projects with multiple developers. 

## tldr 
 
> A PHP static analysis tool to discover bugs in code.
> More information: <https://github.com/phpstan/phpstan>.

- Display available options for analysis:

`phpstan analyse --help`

- Analyze the specified space-separated directories:

`phpstan analyse {{path/to/directory}}`

- Analyze a directory using a configuration file:

`phpstan analyse {{path/to/directory}} --configuration {{path/to/config}}`

- Analyze using a specific rule level (0-7, higher is stricter):

`phpstan analyse {{path/to/directory}} --level {{level}}`

- Specify an autoload file to load before analyzing:

`phpstan analyse {{path/to/directory}} --autoload-file {{path/to/autoload_file}}`

- Specify a memory limit during analysis:

`phpstan analyse {{path/to/directory}} --memory-limit {{memory_limit}}`
