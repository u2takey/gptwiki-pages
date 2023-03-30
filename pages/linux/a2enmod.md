# a2enmod 
## chatgpt 
a2enmod is a command used in Linux/Unix systems to enable an Apache module. 

Apache modules are pieces of software that can be added to the Apache web server to add additional functionality. Examples of modules include mod_rewrite for URL rewriting, mod_ssl for encryption, and mod_php for integrating PHP scripts.

The command syntax for a2enmod is as follows:

```
a2enmod [module-name]
```

Where [module-name] is the name of the module you wish to enable. 

When executed, the a2enmod command will create a symbolic link from the module’s configuration file in the /etc/apache2/mods-available directory to the corresponding directory in /etc/apache2/mods-enabled directory. This will make the module active the next time the Apache server is started or restarted.

Note that a2enmod must be executed as the root user or with sudo privileges. Also, not all modules are available by default, and some may require additional installation and configuration before they can be enabled. 

## tldr 
 
> Enable an Apache module on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2enmod.8.en.html>.

- Enable a module:

`sudo a2enmod {{module}}`

- Don't show informative messages:

`sudo a2enmod --quiet {{module}}`
