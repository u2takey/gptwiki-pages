# lebab 
## chatgpt 
Lebab is a command line tool that is used to transform ES5 syntax into more modern ES6+ syntax. It can be used to convert code written in old JavaScript syntax into more modern, cleaner, and simpler ES6+ syntax. Lebab is easy to use and can improve your code readability, maintainability, and reduce the chances of errors.

Some examples of transformations that Lebab can perform include:

- Converting `var` to `let` and `const` declarations
- Converting old-style `function () {}` declarations to arrow functions
- Converting `arguments` object to the rest operator
- Converting string concatenation to template literals
- Converting `.bind()` to arrow functions or default parameter values

Lebab can be installed globally using the npm package manager with the command:

```
npm install -g lebab
```

After installation, Lebab can be used to transform JavaScript files from the command line. For example, to transform a file called `oldcode.js` into more modern ES6+ syntax, you would run:

```
lebab oldcode.js --replace
```

The `--replace` option tells Lebab to overwrite the original file with the transformed code. If you don't want to overwrite the original file, you can use the `--out-file` option to specify a new file to write the transformed code to.

Lebab also provides a number of options to customize the transformations it performs. These options can be passed in on the command line or specified in a configuration file. Some of the options available include:

- `--transform`: Specifies which transformation(s) to perform (e.g. `let`, `arrow`, `arg-spread`, etc.)
- `--ignore`: Specifies which files to ignore during transformation
- `--verbose`: Displays additional information during the transformation process

Overall, Lebab is a powerful tool that can help you modernize your JavaScript code and improve its overall quality. 

## tldr 
 
> A JavaScript modernizer for transpiling code to ES6/ES7.
> Transformations must be provided for all examples.
> More information: <https://github.com/lebab/lebab>.

- Display a list of the available transformations:

`lebab --help`

- Transpile using one or more comma-separated transformations:

`lebab --transform {{transformation}}`

- Transpile a file to `stdout`:

`lebab {{path/to/input_file}}`

- Transpile a file to the specified output file:

`lebab {{path/to/input_file}} --out-file {{path/to/output_file}}`

- Replace all `.js` files in-place in the specified directory, glob or file:

`lebab --replace {{directory|glob|file}}`
