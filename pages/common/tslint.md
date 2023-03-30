# tslint 
## chatgpt 
TSLint is a static analysis tool that checks TypeScript code for readability, maintainability, and functionality errors. 

When executed, the `tslint` command reads the source code of a TypeScript project, analyzes it, and generates a report highlighting problems that violate the set rules specified in the `tslint.json` configuration file. 

`tslint` can be run from the command prompt or integrated into a continuous integration tool or code editor. The command can take a variety of options and flags to customize the behavior of the linting process, such as specifying a configuration file, ignoring specific files or directories, outputting results in various formats, or fixing issues automatically.

For example, to run `tslint` on a file called `myFile.ts` using a custom configuration file called `myTslint.json` and output the results in JSON format, the command can be executed as follows:

```
tslint --config myTslint.json --format json myFile.ts
```

This will analyze `myFile.ts` according to the rules specified in `myTslint.json` and display the results in JSON format. 

Overall, `tslint` is a powerful tool that helps TypeScript developers write high-quality code, find and fix potential issues, and increase the maintainability and readability of their projects. 

## tldr 
 
> A pluggable linting utility for TypeScript.
> More information: <https://palantir.github.io/tslint>.

- Create TSLint config:

`tslint --init`

- Lint on a given set of files:

`tslint {{filename}}.js {{filename1}}.js`

- Fix lint issues:

`tslint --fix`

- Lint with the config file in the project root:

`tslint --project {{path/to/project_root}}`
