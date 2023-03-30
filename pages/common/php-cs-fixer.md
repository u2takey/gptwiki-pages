# PHP-CS-Fixer 
## chatgpt 
PHP-CS-Fixer is a command-line tool and PHP library that can be used to automatically fix PHP coding standards issues within your codebase. It scans your PHP files and identifies issues such as incorrect indentation, braces placement, whitespace, line endings, etc. and automatically applies fixes to correct them according to the rules and standards defined by the PSR and Symfony. 

The tool is highly customizable and supports a wide range of configuration options that allow you to tailor its behavior according to your specific needs. You can configure the tool to run on a single file or an entire codebase, specify which coding standards to apply, and exclude specific directories, files or rules from being checked. 

To use PHP-CS-Fixer, you need to install it first by running the following command in your terminal:

```
composer require friendsofphp/php-cs-fixer --dev
```

Once installed, you can run the tool by running the following command:

```
./vendor/bin/php-cs-fixer fix /path/to/directory-or-file
```

This will scan the specified directory or file, identify any coding standards issues, and automatically apply fixes to correct them. You can also customize the command by using various options and flags such as `--dry-run` to preview the changes without modifying the files, `--rules` to specify the coding standards to apply, and `--exclude` to exclude specific directories or files from being scanned. 

Overall, PHP-CS-Fixer is a powerful tool that can help you maintain a clean and consistent PHP codebase, which is crucial for improving code readability, maintainability, and reducing bugs and errors. 

## tldr 
 
> Automatic coding style fixer for PHP.
> More information: <https://github.com/FriendsOfPHP/PHP-CS-Fixer>.

- Execute code style fixing in the current directory:

`php-cs-fixer fix`

- Execute code style fixing for a specific directory:

`php-cs-fixer fix {{path/to/directory}}`

- Execute code style linting without applying changes:

`php-cs-fixer fix --dry-run`

- Execute code style fixes using specific rules:

`php-cs-fixer fix --rules={{rules}}`

- Display the rules that have been applied:

`php-cs-fixer fix --verbose`

- Output the results in a different format:

`php-cs-fixer fix --format={{txt|json|xml|checkstyle|junit|gitlab}}`

- Display files that require fixing:

`php-cs-fixer list-files`

- Describe a rule or ruleset:

`php-cs-fixer describe {{rule}}`
