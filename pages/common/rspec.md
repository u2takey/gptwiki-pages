# rspec 
## chatgpt 
`rspec` is a command-line tool that is typically used for running automated tests written in Ruby code.

When executed, the `rspec` command will search the current directory and its subdirectories for any files with names that match the pattern `*_spec.rb`. These files contain Ruby code that defines various types of automated tests, such as unit tests, integration tests, and acceptance tests.

For each of these test files, `rspec` will read the code and execute the tests defined within it. The output of the tests will be displayed in the command-line interface, along with information about which tests passed or failed.

Some common options for the `rspec` command include:

- `-f` or `--format`: set the format of the test output (e.g. `documentation`, `progress`, `html`)
- `-r` or `--require`: specify additional files or directories to load before running the tests
- `-t` or `--tag`: run only tests with certain tags (e.g. `@slow`, `@focus`, `@smoke`)
- `-e` or `--example`: run only tests that match a specific string or regular expression (e.g. `-e "User login"`) 

## tldr 
 
> Behavior-driven development testing framework written in Ruby to test Ruby code.
> More information: <https://rspec.info>.

- Initialize an .rspec config and a spec helper file:

`rspec --init`

- Run all tests:

`rspec`

- Run a specific directory of tests:

`rspec {{path/to/directory}}`

- Run a specific test file:

`rspec {{path/to/file}}`

- Run multiple test files:

`rspec {{path/to/file1}} {{path/to/file2}}`

- Run a specific test in a file (e.g. the test starts on line 83):

`rspec {{path/to/file}}:{{83}}`

- Run specs with a specific seed:

`rspec --seed {{seed_number}}`
