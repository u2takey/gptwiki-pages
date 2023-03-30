# shellcheck 
## chatgpt 
`shellcheck` is a command that provides static code analysis for shell scripts. It checks for common errors, bugs, and vulnerabilities in the script and helps the developer to identify them before executing the script. 

When executed, `shellcheck` reads the shell script and checks for syntax errors, variable and argument issues, quoting problems, and security issues. If a problem is detected, it produces an error message indicating the type of issue and its location in the script. It also suggests solutions to fix the problem.

The `shellcheck` command is used by developers and programmers during the development process to ensure that their shell scripts are error-free and secure. It can be used within automated testing processes to detect and alert errors in shell scripts during continuous integration and deployment processes. 

## tldr 
 
> Shell script static analysis tool.
> Check shell scripts for errors, usage of deprecated/insecure features, and bad practices.
> More information: <https://www.shellcheck.net>.

- Check a shell script:

`shellcheck {{path/to/script.sh}}`

- Check a shell script interpreting it as the specified shell dialect (overrides the shebang at the top of the script):

`shellcheck --shell {{sh|bash|dash|ksh}} {{path/to/script.sh}}`

- Ignore one or more error types:

`shellcheck --exclude {{SC1009,SC1073}} {{path/to/script.sh}}`

- Also check any sourced shell scripts:

`shellcheck --checked-sourced {{path/to/script.sh}}`

- Display output in the specified format (defaults to `tty`):

`shellcheck --format {{tty|checkstyle|diff|gcc|json|json1|quiet}} {{path/to/script.sh}}`

- Enable one or more optional checks:

`shellcheck --enable={{add-default-case|avoid-nullary-conditions}}`

- List all available optional checks that are disabled by default:

`shellcheck --list-optional`
