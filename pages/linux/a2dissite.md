# a2dissite 
## chatgpt 
a2dissite is a command used in Apache web server to disable a site by removing the site configuration file from the sites-enabled directory. 

More specifically, when a new site is added to Apache, a configuration file for that site is created in the /etc/apache2/sites-available directory. This configuration file contains the necessary settings and directives for the site to function properly. However, this file is not automatically enabled for use by Apache.

To enable a site, a symbolic link to the configuration file is created in the /etc/apache2/sites-enabled directory. This tells Apache to load and use the site configuration.

On the other hand, to disable a site, a2dissite command is used. This command essentially removes the symbolic link that was previously created in the sites-enabled directory, effectively disabling the site. The original configuration file in the sites-available directory remains intact and is not deleted.

Overall, the a2dissite command is used to disable a site in Apache by removing its symbolic link from the sites-enabled directory, and it can be paired with the a2ensite command to enable the same or different site. 

## tldr 
 
> Disable an Apache virtual host on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2dissite.8.en.html>.

- Disable a virtual host:

`sudo a2dissite {{virtual_host}}`

- Don't show informative messages:

`sudo a2dissite --quiet {{virtual_host}}`
