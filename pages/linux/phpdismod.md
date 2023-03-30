# phpdismod 
## chatgpt 
phpdismod is a Linux command that is used to disable a specific PHP module. It is a part of the PHP extension management tool set provided by the PHP interpreter. 

When a PHP module is installed, it needs to be loaded by the PHP interpreter for it to function. However, not all modules are required by every application or website. Sometimes, a module may conflict with other installed software, or it may not be needed by the web application. 

In such cases, disabling the module using phpdismod can help in preventing any potential conflicts and saving resources. 

The syntax of phpdismod is as follows:

phpdismod [OPTIONS] MODULE_NAME

Here, MODULE_NAME is the name of the PHP module that you want to disable. 

Some of the common options that can be used with phpdismod command are:

- -h or --help: Displays the help message for the command.
- -v or --version: Displays the version information for the command.
- -s or --sapi: Specifies the php SAPI module to use (e.g cgi or fpm).
- -f or --force: Forces the command to execute without asking for confirmation.

To disable a PHP module using phpdismod, you need to be logged in as a superuser or have sudo permissions. Once you have the necessary permissions, you can run the following command:

sudo phpdismod MODULE_NAME

This will disable the specified PHP module and it will no longer load when the PHP interpreter is called. You may need to restart any running PHP processes for the change to take effect. 

Overall, phpdismod command is a useful tool in managing PHP modules and ensuring that only the necessary modules are loaded, reducing the risk of conflicts and improving the overall performance of the web application. 

## tldr 
 
> Disable PHP extensions on Debian-based OSes.
> More information: <https://salsa.debian.org/php-team/php-defaults>.

- Disable the JSON extension for every SAPI of every PHP version:

`sudo phpdismod {{json}}`

- Disable the JSON extension for PHP 7.3 with the cli SAPI:

`sudo phpdismod -v {{7.3}} -s {{cli}} {{json}}`
