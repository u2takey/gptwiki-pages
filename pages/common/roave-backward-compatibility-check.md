# roave-backward-compatibility-check 
## chatgpt 
`roave-backward-compatibility-check` is a command-line tool used to check backward compatibility of PHP code between two versions. The tool checks for any changes in the code that may break its compatibility with a previous version.

The command takes two arguments: the first argument is the path to the old version of the code, while the second argument is the path to the new version of the code. The tool analyzes the code changes between the two versions and generates an HTML report of any backward compatibility issues it finds.

Roave-backward-compatibility-check can also be used as a Composer plugin, allowing you to integrate it into your project to ensure that code changes do not introduce backward compatibility issues.

The tool checks for changes in interfaces, methods, and class properties, among other things. It also checks for changes in function signatures, which can cause issues for calling code that expects a specific signature.

Overall, roave-backward-compatibility-check helps maintain the stability of code and ensures that updates and changes to the codebase do not introduce any critical issues that may impact the end-users. 

## tldr 
 
> A tool that can be used to verify backward compatibility breaks between two versions of a PHP library.
> More information: <https://github.com/Roave/BackwardCompatibilityCheck>.

- Check for breaking changes since the last tag:

`roave-backward-compatibility-check`

- Check for breaking changes since a specific tag:

`roave-backward-compatibility-check --from={{git_reference}}`

- Check for breaking changes between the last tag and a specific reference:

`roave-backward-compatibility-check --to={{git_reference}}`

- Check for breaking changes and output to Markdown:

`roave-backward-compatibility-check --format=markdown > {{results.md}}`
