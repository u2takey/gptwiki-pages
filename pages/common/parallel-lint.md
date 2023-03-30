# parallel-lint 
## chatgpt 
Parallel-lint is a command used for linting PHP code, which means that it checks for potential errors, bugs, or coding conventions violations in the code. The command is executed in a parallel manner, which makes it faster compared to running it on a single core. 

The parallel-lint command typically requires specifying a directory or file path to be analyzed. It recursively searches for all PHP files and runs them through the linting process. 

Some common options used with parallel-lint include:

- `--exclude` : Specifies a pattern to exclude files matching that pattern from being analyzed.
- `--no-progress` : Disables the progress bar displayed during the analysis.
- `--shell` : Runs the linter as a shell command.
- `--php` : Specifies the PHP executable to be used to run the linter. 

The output of parallel-lint includes a summary of the analyzed files, the number of errors and warnings, and the execution time. The report also lists the specific files and lines that contain any issues found during the analysis. 

Parallel-lint is a useful command during software development to ensure that the code adheres to best practices, standards, and avoid potential issues that may arise in production. 

## tldr 
 
> A tool to check the syntax of PHP files in parallel.
> More information: <https://github.com/JakubOnderka/PHP-Parallel-Lint>.

- Lint a specific directory:

`parallel-lint {{path/to/directory}}`

- Lint a directory using the specified number of parallel processes:

`parallel-lint -j {{processes}} {{path/to/directory}}`

- Lint a directory, excluding the specified directory:

`parallel-lint --exclude {{path/to/excluded_directory}} {{path/to/directory}}`

- Lint a directory of files using a comma-separated list of extension(s):

`parallel-lint -e {{php,html,phpt}} {{path/to/directory}}`

- Lint a directory and output the results as JSON:

`parallel-lint --json {{path/to/directory}}`

- Lint a directory and show Git Blame results for rows containing errors:

`parallel-lint --blame {{path/to/directory}}`
