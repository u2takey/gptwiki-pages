# nginx 
## chatgpt 
nginx is a web server software that can be used to serve static and dynamic content over the World Wide Web. It is also used as a reverse proxy, load balancer, and HTTP cache. The command "nginx" is used to start, stop, reload, and test the configuration file of the software.

Here are some examples of how to use the "nginx" command:

1. Starting nginx:
To start the nginx web server, type the following command:

$ sudo systemctl start nginx

This will start the nginx service and make it available for incoming requests.

2. Stopping nginx:
To stop the nginx service, type the following command:

$ sudo systemctl stop nginx

This will stop the nginx service and all incoming requests will be rejected.

3. Reloading nginx configuration:
If you make any changes to the nginx configuration file, you need to reload the server configuration using the following command:

$ sudo systemctl reload nginx

This will reload the nginx configuration file and apply the changes to the server.

4. Testing nginx configuration:
To test the nginx configuration file, type the following command:

$ sudo nginx -t

This will check the syntax of the nginx configuration file, report any errors, and exit. If there are no errors reported, the configuration file is valid and ready for use.

Overall, the "nginx" command is an essential tool for managing the nginx web server and ensuring that it is running smoothly. 

## tldr 
 
> Nginx web server.
> More information: <https://nginx.org/en/>.

- Start server with the default config file:

`nginx`

- Start server with a custom configuration file:

`nginx -c {{configuration_file}}`

- Start server with a prefix for all relative paths in the configuration file:

`nginx -c {{configuration_file}} -p {{prefix/for/relative/paths}}`

- Test the configuration without affecting the running server:

`nginx -t`

- Reload the configuration by sending a signal with no downtime:

`nginx -s reload`
