# ionic 
## chatgpt 
Ionic is a command-line interface (CLI) tool and a framework for creating hybrid mobile applications using web technologies such as HTML, CSS, and JavaScript. The ionic command is the main command used in the Ionic CLI and is used to perform various tasks such as creating new projects, generating new components, serving the application locally for testing, building the application, and deploying it to various platforms.

When executed, the ionic command opens up the CLI and provides a list of available commands and options that can be used to carry out specific tasks. Some of the available commands include:

- start: Creates a new Ionic project with the recommended starter template
- generate: Creates new components such as pages, directives, services, and pipes
- serve: Starts a local dev server to test the application on the browser
- build: Builds the application for production
- cordova: Enables integration with Cordova for access to native device functionalities
- cap: Enables integration with Capacitor for building native mobile applications using web technologies

The ionic command can also be used with various options such as specifying the target platform, the output directory, and other project configuration options. In summary, the ionic command is the primary tool used for developing, testing, building, and deploying Ionic applications. 

## tldr 
 
> A framework to build hybrid mobile apps.
> More information: <https://ionicframework.com/docs/cli>.

- Create a new project:

`ionic start`

- Start a local dev server for app dev/testing:

`ionic serve`

- Generate new app component, directive, page, pipe, provider or tabs:

`ionic g {{page}}`

- Show versions of Ionic, Cordova, environment, etc.:

`ionic info`

- Run app on an Android/iOS device:

`ionic cordova run {{android|ios}} --device`

- Check the health of an Ionic app:

`ionic doctor {{check}}`
