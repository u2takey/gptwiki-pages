# composer-require-checker 
## chatgpt 
Composer require checker is a command-line tool that scans your project's dependencies and identifies whether you are using any wrong or outdated versions.

When you enter the "composer-require-checker" command, the tool loads the project's composer.json file and its dependencies. It then compares each package in the composer.json file with the latest available version in the Packagist repository. It identifies whether any package version mismatches, i.e., whether a package is updated or not.

If a package's version is outdated or wrong, the composer-require-checker tool gives a detailed report on the package with the installed version, the latest available version, and the differences between the two versions. This helps you identify whether you need to update the package or not.

By using the composer-require-checker command, you can keep your project's dependencies updated, which ultimately benefits your application's performance, stability, and security. 

## tldr 
 
> A CLI tool to analyze Composer dependencies for soft dependencies.
> More information: <https://github.com/maglnet/ComposerRequireChecker>.

- Analyze a Composer JSON file:

`composer-require-checker check {{path/to/composer.json}}`

- Analyze a Composer JSON file with a specific configuration:

`composer-require-checker check --config-file {{path/to/config.json}} {{path/to/composer.json}}`
