# a2disconf 
## chatgpt 
a2disconf is a command used in Apache web server to disable a configuration file. This command is used to disable any existing configuration file for the Apache HTTP server. 

The "a2disconf" stands for Apache 2.0 Disable Config. “a2disconf” is a script created to simplify the process of disabling Apache configuration files. This command disables the configuration file without physically deleting the configuration file.

When you run the a2disconf command, it will check if the specified configuration file exists in the /etc/apache2/sites-available/ directory. If the configuration file exists, the command will create a symlink in /etc/apache2/sites-enabled/ pointing to /etc/apache2/sites-available/ with the same name as the configuration file. 

Once the symlink is created, the configuration file is disabled, and the Apache web server will not read or load the disabled configuration file. This means that any changes made to the disabled configuration file will not have an effect on the Apache web server.

To summarize, a2disconf is a command used to disable any existing configuration file for the Apache HTTP server. This command will create a symlink in /etc/apache2/sites-enabled/ pointing to /etc/apache2/sites-available/ with the same name as the configuration file. This symlink will disable the configuration file, and the Apache web server won't read or load it. 

## tldr 
 
> Disable an Apache configuration file on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2disconf.8.en.html>.

- Disable a configuration file:

`sudo a2disconf {{configuration_file}}`

- Don't show informative messages:

`sudo a2disconf --quiet {{configuration_file}}`
