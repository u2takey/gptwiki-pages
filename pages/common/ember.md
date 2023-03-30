# ember 
## chatgpt 
`ember` is a command-line interface (CLI) tool used for developing web applications with Ember.js, a front-end JavaScript framework. The `ember` command is used to perform various tasks related to creating, building, and testing Ember.js applications.

Here are some of the commonly used sub-commands of `ember`:

- `new`: Creates a new Ember.js app with the specified name and options.
- `generate`: Generates new files and structures for the app, such as components, routes, controllers, and templates.
- `serve`: Starts a local development server that serves the app and reloads it automatically when changes are made.
- `test`: Runs test suites for the app or specific modules.
- `build`: Builds the app for production deployment by concatenating, minifying, and optimizing the code.

Some additional flags and options that can be used with the `ember` command include:

- `--environment`: Specifies the environment (e.g. development, test, production) for the app.
- `--port`: Specifies the port number for the server to listen on.
- `--proxy`: Specifies a proxy URL for API requests during development.
- `--watcher`: Specifies the file watcher to use (e.g. polling, watchman, livereload).
- `--verbose`: Shows detailed output during command execution.

In summary, the `ember` command is a powerful tool that simplifies development with Ember.js by automating common tasks and providing a consistent interface for project management. 

## tldr 
 
> The Ember.js command-line utility.
> Used for creating and maintaining Ember.js applications.
> More information: <https://cli.emberjs.com>.

- Create a new Ember application:

`ember new {{my_new_app}}`

- Create a new Ember addon:

`ember addon {{my_new_addon}}`

- Build the project:

`ember build`

- Build the project in production mode:

`ember build -prod`

- Run the development server:

`ember serve`

- Run the test suite:

`ember test`

- Run a blueprint to generate something like a route or component:

`ember generate {{type}} {{name}}`

- Install an ember-cli addon:

`ember install {{name_of_addon}}`
