# react-native start 
## chatgpt 
The "react-native start" command is used to start the React Native development server. This command is usually executed from the root directory of a React Native project.

Once executed, this command will start the development server and make the project available to simulators or devices for development and testing purposes. The development server provides many features such as hot module reloading, debugging, and logging.

When the server is started, a Metro server instance will also be launched which will take care of building the JavaScript bundle for the application. The Metro server will continue running until the developer stops the server by pressing Ctrl + C.

Overall, the "react-native start" command is the starting point for developing a React Native application and is an essential component of the React Native development process. 

## tldr 
 
> Command-line tools to start the React Native server.
> More information: <https://github.com/react-native-community/cli/blob/master/docs/commands.md#start>.

- Start the server that communicates with connected devices:

`react-native start`

- Start the metro bundler with a clean cache:

`react-native start --reset-cache`

- Start the server in a custom port (defaults to 8081):

`react-native start --port {{3000}}`

- Start the server in verbose mode:

`react-native start --verbose`

- Specify the maximum number of workers for transforming files (default is the number of CPU cores):

`react-native start --max-workers {{count}}`

- Disable interactive mode:

`react-native start --no-interactive`
