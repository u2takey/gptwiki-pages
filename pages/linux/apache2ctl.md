# apache2ctl 
## chatgpt 
The "apache2ctl" command is used in the Apache web server to perform various administrative tasks. Here are some of the main options the command supports:

- start: starts the Apache web server
- stop: stops the Apache web server
- restart: restarts the Apache web server
- status: displays the current status of the Apache web server
- graceful: gracefully restarts the Apache web server, allowing current connections to finish before restarting
- configtest: checks the syntax of the Apache configuration file before starting the web server

In general, the "apache2ctl" command is used to control the operation of the Apache web server, including starting, stopping, and restarting the server, checking its status, and testing its configuration file. It is typically used by system administrators who manage web servers running Apache. 

## tldr 
 
> The CLI tool to administrate HTTP web server Apache.
> This command comes with Debian based OSes, for RHEL based ones see `httpd`.
> More information: <https://manpages.debian.org/latest/apache2/apache2ctl.8.en.html>.

- Start the Apache daemon. Throw a message if it is already running:

`sudo apache2ctl start`

- Stop the Apache daemon:

`sudo apache2ctl stop`

- Restart the Apache daemon:

`sudo apache2ctl restart`

- Test syntax of the configuration file:

`sudo apache2ctl -t`

- List loaded modules:

`sudo apache2ctl -M`
