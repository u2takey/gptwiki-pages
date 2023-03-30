# phpenmod 
## chatgpt 
The `phpenmod` command is used in Linux-based systems to enable a PHP module. Here's a detailed explanation of the command:

Syntax:

```
sudo phpenmod <module_name>
```

The `phpenmod` command is generally used with the `sudo` prefix since it requires administrative privileges to make changes to the system.

Arguments:

- `<module_name>`: This is the name of the PHP module that you want to enable.

Example:

```
sudo phpenmod gd
```

This example will enable the GD extension for PHP.

Explanation:

The `phpenmod` command is part of the `php-common` package, which is commonly installed in Linux-based systems. This package contains various utilities that are used to manage PHP configurations.

When you run the `phpenmod` command with a module name, it searches for the corresponding configuration file in the `/etc/php/<version>/mods-available` directory. If the file is found, it creates a symbolic link to that file in the `/etc/php/<version>/cli/conf.d` and `/etc/php/<version>/apache2/conf.d` directories, which are used by the command-line interface and the Apache web server, respectively.

This symbolic link allows the module to be loaded into PHP when it is executed by the server or the command line. By default, all modules listed in the configuration files (`/etc/php/<version>/conf.d/*.ini`) are loaded when PHP is executed. However, if a module is not included in any configuration file, it will not be loaded.

In conclusion, the `phpenmod` command helps enable PHP modules in a Linux-based system by creating a symbolic link to the configuration file that is necessary for the module to function properly. 

## tldr 
 
> Enable PHP extensions on Debian-based OSes.
> More information: <https://salsa.debian.org/php-team/php-defaults>.

- Enable the JSON extension for every SAPI of every PHP version:

`sudo phpenmod {{json}}`

- Enable the JSON extension for PHP 7.3 with the cli SAPI:

`sudo phpenmod -v {{7.3}} -s {{cli}} {{json}}`
