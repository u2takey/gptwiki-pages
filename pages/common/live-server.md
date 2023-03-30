# live-server 
## chatgpt 
The `live-server` command is a tool that allows you to create a local development server and serves up your web app or website on the fly. When you run the `live-server` command, it starts a new web server on your local system and serves your web app, website, or other files to your browser using that local server.

Some key features of `live-server` include:

- Automatic browser refresh: Whenever you make changes to your code or files, `live-server` will automatically reload the browser to show you the updated content. This makes development faster and more efficient, as you don't need to manually hit refresh every time you make changes.
- Static file support: `live-server` can serve up static files such as HTML, CSS, and JavaScript files, as well as other types of files that are commonly used in web development.
- Customizable settings: You can configure `live-server` to use different options and settings, such as which port to use, which directory to serve files from, and more.

To use `live-server`, you need to first install it on your system using a package manager such as npm. Once it's installed, you can run the `live-server` command from the command line along with any options or settings you want to use. For example, you might run `live-server --port=8080` to start the server on port 8080, or `live-server --entry-file=index.html` to specify that the server should serve the `index.html` file as the default entry point for your web app or site. 

## tldr 
 
> A simple development HTTP server with live reload capability.
> More information: <https://github.com/tapio/live-server>.

- Serve an `index.html` file and reload on changes:

`live-server`

- Specify a port (default is 8080) from which to serve a file:

`live-server --port={{8081}}`

- Specify a given file to serve:

`live-server --open={{about.html}}`

- Proxy all requests for ROUTE to URL:

`live-server --proxy={{/}}:{{http:localhost:3000}}`
