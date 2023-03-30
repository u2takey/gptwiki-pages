# phpenv 
## chatgpt 
phpenv is a command for managing multiple versions of PHP on a single machine. 

When working with multiple applications or projects that require different versions of PHP, phpenv allows you to switch between them easily. 

Some of the main functions of phpenv include:

1. Installing new versions of PHP
2. Listing installed versions of PHP
3. Switching between versions of PHP
4. Setting the global PHP version
5. Customizing PHP configuration options

By using phpenv, you can ensure that each project or application is using the correct version of PHP without any conflicts. It simplifies the process of managing multiple PHP installations on a single machine. 

## tldr 
 
> A PHP version manager for development purposes.
> More information: <https://github.com/phpenv/phpenv>.

- Install a PHP version globally:

`phpenv install {{version}}`

- Refresh shim files for all PHP binaries known to `phpenv`:

`phpenv rehash`

- List all installed PHP versions:

`phpenv versions`

- Display the currently active PHP version:

`phpenv version`

- Set the global PHP version:

`phpenv global {{version}}`

- Set the local PHP version, which overrides the global version:

`phpenv local {{version}}`

- Unset the local PHP version:

`phpenv local --unset`
