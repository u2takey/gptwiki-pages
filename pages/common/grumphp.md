# grumphp 
## chatgpt 
`GrumPHP` is an open source PHP code quality tool that checks the code for syntax errors, code standards, and other issues. It can be used as a pre-commit hook for Git, which means that it runs automatically before committing the code, and can prevent developers from committing low-quality code to the repository. 

To use `GrumPHP`, the first step is to install it using `Composer`. Once installed, you can run the `grumphp` command to start configuring the tool. The basic configuration would include specifying the directories and files to include or exclude from the checks, as well as defining the rules and standards to apply. 

Some of the features of `GrumPHP` include:

- Running the PHP built-in linter to detect syntax errors
- Running third-party tools like `phpcs` (PHP Code Sniffer), `phpmd` (PHP Mess Detector), and `php-cs-fixer` to enforce coding standards, detect potential bugs, and ensure code quality
- Configuring custom rules and commands using `Symfony` and `JSON` structures
- Integration with popular PHP frameworks like `Symfony`, `Laravel`, and `Zend`

Overall, `GrumPHP` is a powerful tool that can help improve the quality, consistency, and reliability of your PHP codebase. 

## tldr 
 
> A PHP Composer plugin that enables source code quality checks.
> More information: <https://github.com/phpro/grumphp>.

- Register the Git hooks:

`grumphp git:init`

- Trigger the pre-commit hook manually:

`grumphp git:pre-commit`

- Check every versioned file:

`grumphp run`
