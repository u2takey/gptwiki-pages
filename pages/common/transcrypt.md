# transcrypt 
## chatgpt 
Transcrypt is a Python to JavaScript transpiler, which means it translates Python code into JavaScript code. 

The basic syntax of the transcrypt command goes as follows: 

```bash
transcrypt [options] files
```

- `transcrypt`: This is the name of the command that invokes the Transcrypt transpiler.
- `[options]`: This indicates that there may be additional flags or arguments to configure the behavior of the command.
- `files`: This specifies the name of the Python file(s) you want to transpile into JavaScript.

Some common options include:

- `-b`: This is short for `--browser`, which specifies that the output should be optimized for running in a web browser.
- `-m`: This is short for `--map`, which generates source maps to help with debugging.
- `-n`: This is short for `--nomin`, which disables minimization of the output.
- `-e`: This is short for `--esvers`, which lets you specify the EcmaScript version to target.

Overall, the `transcrypt` command is used to convert Python code into JavaScript code, making it possible to run Python code in places where only JavaScript is supported, such as web browsers. 

## tldr 
 
> Transparently encrypt files within a Git repository.
> More information: <https://github.com/elasticdog/transcrypt>.

- Initialize an unconfigured repository:

`transcrypt`

- List the currently encrypted files:

`git ls-crypt`

- Display the credentials of a configured repository:

`transcrypt --display`

- Initialize and decrypt a fresh clone of a configured repository:

`transcrypt --cipher={{cipher}}`

- Rekey to change the encryption cipher or password:

`transcrypt --rekey`
