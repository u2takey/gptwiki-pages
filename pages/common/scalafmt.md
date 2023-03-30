# scalafmt 
## chatgpt 
The 'scalafmt' command is a tool used for formatting Scala code. When developers write code using Scala, they might have different coding styles and formatting preferences. As a result, it can be challenging to maintain a consistent coding style across a codebase or project.

The 'scalafmt' command helps in solving this problem by formatting Scala code automatically based on specified style guidelines. When run on a file or directory, 'scalafmt' scans the code and reformats it according to the specified style.

The tool works based on a configuration file, which can be modified to reflect the desired style guidelines. The configuration file specifies the indentation style, maximum line length, and other formatting rules. Developers can choose to adopt an existing configuration file or modify an existing one to suit their preferences.

Overall, the 'scalafmt' command improves the readability, consistency, and maintainability of Scala code, and is a useful tool in Scala development. 

## tldr 
 
> Code formatter for Scala.
> Configurations are stored in the `.scalafmt.conf` file.
> More information: <https://scalameta.org/scalafmt>.

- Reformat all `.scala` files in the current directory recursively:

`scalafmt`

- Reformat specific files or directories with a custom formatting configuration:

`scalafmt --config {{path/to/.scalafmt.conf}} {{path/to/file_or_directory}} {{path/to/file_or_directory}} {{...}}`

- Check if files are correctly formatted, returning `0` if all files respect the formatting style:

`scalafmt --config {{path/to/.scalafmt.conf}} --test`

- Exclude files or directories:

`scalafmt --exclude {{path/to/file_or_directory}} {{...}}`

- Format only files that were edited against the current Git branch:

`scalafmt --config {{path/to/.scalafmt.conf}} --mode diff`
