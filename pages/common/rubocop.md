# rubocop 
## chatgpt 
RuboCop is a static code analysis tool that enforces the Ruby community's style guide (also known as the Ruby Style Guide) and detects code offenses and errors in Ruby code.

When the command `rubocop` is executed in a Ruby development environment or in the terminal, it will analyze the codebase in the current directory or specified directory, and display a list of code offenses or errors, as well as suggestions for improving the code's style.

RuboCop can be configured with custom rules and configuration files to fit individual or team-specific style guidelines. This is done by creating a `.rubocop.yml` file in the project directory and configuring the tool to operate based on the custom rules and guidelines.

By using RuboCop in a project, automated code analysis can help improve code quality, consistency, and maintainability by enforcing a common style and detecting common Ruby coding mistakes. 

## tldr 
 
> Lint Ruby files.
> More information: <https://docs.rubocop.org/rubocop/usage/basic_usage.html>.

- Check all files in the current directory (including subdirectories):

`rubocop`

- Check one or more specific files or directories:

`rubocop {{path/to/file}} {{path/to/directory}}`

- Write output to file:

`rubocop --out {{path/to/file}}`

- View list of cops (linter rules):

`rubocop --show-cops`

- Exclude a cop:

`rubocop --except {{cop_1}} {{cop_2}}`

- Run only specified cops:

`rubocop --only {{cop_1}} {{cop_2}}`

- Auto-correct files (experimental):

`rubocop --auto-correct`
