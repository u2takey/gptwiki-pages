# a2dismod 
## chatgpt 
a2dismod is a command used in Linux-based operating systems to disable a module (or a specific part of a program) for the Apache web server. When a module is disabled, it is no longer loaded or executed by the web server.

The command a2dismod is a part of the Apache web server's management tool called Apache2ctl. To use it, the user has to either have administrative privileges or use the sudo command to run as an administrator.

The syntax for the command is:

sudo a2dismod module_name

Here, module_name is the name of the module that needs to be disabled. For example, if the user wants to disable the mod_php module, the command will be:

sudo a2dismod mod_php

Once the command is executed, the module will be disabled, and the user will receive a confirmation message on their terminal.

It is essential to note that disabling a module may affect the web server's functionality and the user should have a good understanding of the module before deciding to disable it. The user can enable the module again by running the a2enmod command with the module name. 

## tldr 
 
> Disable an Apache module on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2dismod.8.en.html>.

- Disable a module:

`sudo a2dismod {{module}}`

- Don't show informative messages:

`sudo a2dismod --quiet {{module}}`
