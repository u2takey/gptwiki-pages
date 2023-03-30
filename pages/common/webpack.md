# webpack 
## chatgpt 
Webpack is a module bundler for modern JavaScript applications. It takes all the assets and dependencies of a web application (such as JavaScript files, stylesheets, images, etc.) and bundles them into static assets that can be served to a client's web browser. The command "webpack" triggers the bundling process and generates a new set of files that are optimized for serving to clients.

When running the "webpack" command, Webpack reads an application's entry point (e.g., index.js), builds a dependency graph based on the imported modules and assets, and generates an optimized output bundle (e.g., bundle.js). The bundling process includes several steps, such as parsing the input code, transforming it using loaders (e.g., transpiling ES6 to ES5), and optimizing the output code for production.

Webpack has a configuration file (webpack.config.js) where developers can define the bundling behavior, such as entry points, output paths, loaders, plugins, and optimization strategies. By customizing the configuration file, developers can tailor the bundling process to their specific needs and optimize the application's performance.

Overall, the "webpack" command is a crucial step in building modern JavaScript web applications, as it transforms source code and assets into optimized static assets that run efficiently in clients' web browsers. 

## tldr 
 
> Bundle a web project's js files and other assets into a single output file.
> More information: <https://webpack.js.org>.

- Create a single output file from an entry point file:

`webpack {{app.js}} {{bundle.js}}`

- Load CSS files too from the JavaScript file (this uses the CSS loader for `.css` files):

`webpack {{app.js}} {{bundle.js}} --module-bind '{{css=css}}'`

- Pass a config file (with e.g. the entry script and the output filename) and show compilation progress:

`webpack --config {{webpack.config.js}} --progress`

- Automatically recompile on changes to project files:

`webpack --watch {{app.js}} {{bundle.js}}`
