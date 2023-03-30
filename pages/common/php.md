# php 
## chatgpt 
"php" is a command used in the command line interface (CLI) of a computer to execute PHP scripts. PHP is a popular programming language used for web development, command-line scripting, server-side processing of data, and much more. 

When the "php" command is executed in the CLI, it looks for a PHP interpreter installed on the system and uses it to interpret or execute the PHP code. The PHP interpreter reads the code line-by-line, interprets it, and outputs the results.

Some common use cases of the "php" command are:

1. Running a PHP script: You can execute a PHP script by typing "php filename.php" in the CLI.

2. Running a single line of code: You can run a single line of PHP code by typing "php -r 'code here'" in the CLI.

3. Checking the PHP version: You can check the version of PHP installed on your system by typing "php -v" in the CLI.

4. Starting a built-in web server: You can start a built-in web server by typing "php -S localhost:8000" in the CLI.

Overall, the "php" command is an essential tool for PHP programmers and web developers. It allows them to interact with and execute PHP code quickly and efficiently. 

## tldr 
 
> PHP command-line interface.
> More information: <https://php.net>.

- Parse and execute a PHP script:

`php {{path/to/file}}`

- Check syntax on (i.e. lint) a PHP script:

`php -l {{path/to/file}}`

- Run PHP interactively:

`php -a`

- Run PHP code (Notes: Don't use <? ?> tags; escape double quotes with backslash):

`php -r "{{code}}"`

- Start a PHP built-in web server in the current directory:

`php -S {{host:port}}`

- Get a list of installed PHP extensions:

`php -m`

- Display information about the current PHP configuration:

`php -i`

- Display information about a specific function:

`php --rf {{function_name}}`
