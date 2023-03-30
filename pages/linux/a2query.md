# a2query 
## chatgpt 
The command `a2query` is a Linux command used to query various settings or configurations of the Apache 2 web server. It is typically used by system administrators or developers who need to check the status of Apache or other related components.

Here are some of the most common options and use cases for the `a2query` command:

1. `a2query -v`: This option returns the version of Apache 2 installed on the system.

2. `a2query -S`: This option lists all the Virtual Hosts and other settings configured in Apache 2.

3. `a2query -M`: This option lists all the Apache 2 modules currently installed and activated.

4. `a2query -l`: This option lists all the available Apache 2 modules that are available but not yet activated.

5. `a2query -T`: This option tests the Apache 2 configuration files and returns any syntax errors.

Overall, the `a2query` command is a simple and useful tool for checking the status of an Apache 2 web server and its configuration. It can save time for administrators and developers by quickly providing important information that can be used to troubleshoot or optimize the server. 

## tldr 
 
> Retrieve runtime configuration from Apache on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2query.html>.

- List enabled Apache modules:

`sudo a2query -m`

- Check if a specific module is installed:

`sudo a2query -m {{module_name}}`

- List enabled virtual hosts:

`sudo a2query -s`

- Display the currently enabled Multi Processing Module:

`sudo a2query -M`

- Display the Apache version:

`sudo a2query -v`
