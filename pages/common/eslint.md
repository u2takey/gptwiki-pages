# eslint 
## chatgpt 
ESLint is a command-line tool used for analyzing source code to flag programming errors, code smells, and other issues related to coding standards. 

To use the `eslint` command, you need to have the tool installed on your system either globally or locally within a project. Once you have installed or added the eslint dependency, you can open your terminal or command prompt and run the `eslint` command followed by the path to the file or directory you want to scan. 

For example, if you want to lint a file named `index.js`, you can run the command `eslint index.js`. ESLint will analyze the file and report any detected errors or issues following the rules specified in the configuration file for the project.

ESLint provides several command-line options and flags that you can use to customize the way it analyzes your code, including specifying different configuration files, setting environment variables, specifying file globs, and more. 

Overall, the `eslint` command is a powerful tool for improving the quality of your code, making it more maintainable, and ensuring it adheres to coding best practices. 

## tldr 
 
> A pluggable linting utility for JavaScript and JSX.
> More information: <https://eslint.org>.

- Create ESLint config:

`eslint --init`

- Lint on a given set of files:

`eslint {{filename}}.js {{filename1}}.js`

- Fix lint issues:

`eslint --fix`

- Lint with config:

`eslint -c {{path/to/config_file}} {{app/src}}`
