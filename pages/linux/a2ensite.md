# a2ensite 
## chatgpt 
The command "a2ensite" is a Linux command used to enable a specific website in the Apache webserver configuration. 

When a website is created in Apache, it is first added to the configuration file, but it is not active by default. To enable the website, the "a2ensite" command can be used.

The command is used in the following format:
a2ensite < website_name >

The "website_name" should be the name of the configuration file for the website located in the "/etc/apache2/sites-available/" directory.

The "a2ensite" command essentially creates a symbolic link from the "sites-available" directory to the "sites-enabled" directory. This means that the website configuration file is now active and will be used by the Apache webserver to serve the website.

Note that after using the "a2ensite" command, the Apache service needs to be restarted for the changes to take effect. This can be done with the command "sudo service apache2 restart". 

## tldr 
 
> Enable an Apache virtual host on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2ensite.8.en.html>.

- Enable a virtual host:

`sudo a2ensite {{virtual_host}}`

- Don't show informative messages:

`sudo a2ensite --quiet {{virtual_host}}`
