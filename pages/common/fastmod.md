# fastmod 
## chatgpt 
I'm sorry, but as an AI language model, I cannot run commands on a system or a terminal. However, I can provide you with some information on what 'fastmod' is and what it is used for.

'fastmod' is an open-source command-line tool that can be used for making mass modifications to source code files. It can replace strings, delete lines, and insert text into specific positions in multiple files at once. Its main advantage is speed and efficiency, as it can modify thousands of files in seconds, which can be useful for projects with large codebases.

Some of its features include:

- Replacing words or phrases across multiple files
- Deleting lines or entire sections of code
- Extracting text from files
- Inserting text at specific positions within files

To use fastmod, you can install it through NPM (Node Package Manager) using the command: 

```
npm install fastmod -g
```

Once installed, you can start using it by specifying the modifications you want to make in the command line. For example, to replace all instances of 'foo' with 'bar' in all .js files within the 'src' directory and its subdirectories, you can run:

```
fastmod -r -d ./src '*.js' -m 'foo' 'bar'
```

This would replace all instances of 'foo' with 'bar' in all .js files within the 'src' directory and its subdirectories. 

Keep in mind that 'fastmod' is a powerful tool that can make significant changes to your codebase, so it's recommended to use it with caution and test your modifications thoroughly before committing any changes to your repository. 

## tldr 
 
> A fast partial replacement for the codemod tool, replace and replace all in the whole codebase.
> Regexes are matched by Rust regex crate.
> More information: <https://github.com/facebookincubator/fastmod>.

- Replace a regex pattern in all files of the current directory, ignoring files on .ignore and .gitignore:

`fastmod {{regex_pattern}} {{replacement}}`

- Replace a regex pattern in case-insensitive mode in specific files or directories:

`fastmod --ignore-case {{regex_pattern}} {{replacement}} -- {{path/to/file path/to/directory ...}}`

- Replace a regex pattern in a specific directory in files filtered with a case-insensitive glob pattern:

`fastmod {{regex}} {{replacement}} --dir {{path/to/directory}} --iglob {{'**/*.{js,json}'}}`

- Replace for an exact string in .js or .json files:

`fastmod --fixed-strings {{exact_string}} {{replacement}} --extensions {{json,js}}`

- Replace for an exact string without prompt for a confirmation (disables regular expressions):

`fastmod --accept-all --fixed-strings {{exact_string}} {{replacement}}`

- Replace for an exact string without prompt for a confirmation, printing changed files:

`fastmod --accept-all --print-changed-files --fixed-strings {{exact_string}} {{replacement}}`
