# browser-sync 
## chatgpt 
Browser-sync is a command-line tool used to set up local web server and synchronize browser actions across multiple devices by automatically reloading the browser when changes are made to HTML, CSS, or JavaScript files.

When you run the browser-sync command, it starts a local web server and opens your default browser with the web page you specify. Any changes made to the files in the specified directory will prompt a refresh of the browser, allowing you to see the changes instantly. In addition, browser-sync allows you to open the same web page on multiple devices and synchronize the interactions, so you can test the responsiveness of your website on various screen sizes, devices, and browsers.

Some of the configuration options you can set up with browser-sync include specifying the port number, setting up proxy server, enabling or disabling the reloading feature, setting up the log level, and specifying the base directory.

Overall, browser-sync is a powerful tool that can help speed up the web development process by enabling you to see the changes you make to your code in real-time and test your website across multiple devices and browsers. 

## tldr 
 
> Starts local web server that updates browser on file changes.
> More information: <https://browsersync.io/docs/command-line>.

- Start a server from a specific directory:

`browser-sync start --server {{path/to/directory}} --files {{path/to/directory}}`

- Start a server from local directory, watching all CSS files in a directory:

`browser-sync start --server --files '{{path/to/directory/*.css}}'`

- Create configuration file:

`browser-sync init`

- Start browser-sync from config file:

`browser-sync start --config {{config_file}}`
