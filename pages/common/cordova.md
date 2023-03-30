# cordova 
## chatgpt 
Cordova is a command-line interface (CLI) tool used for building hybrid mobile applications. It is an open-source mobile development framework that allows developers to build mobile applications using web technologies such as HTML, CSS, and JavaScript.

The "cordova" command is used to create, build, deploy, and manage Cordova projects. It is the main command used in the development process of a Cordova project.

Some of the common uses of the "cordova" command are:

1. Create a new Cordova project: When creating a new Cordova project, the developer uses the "cordova create" command followed by the project name, package name, and template option to specify the type of application to be created.

2. Add a platform: After creating a Cordova project, the developer uses the "cordova platform add" command followed by the platform name (iOS, Android, Windows, etc.) to add a platform to the project.

3. Build the project: To build the Cordova project, the developer uses the "cordova build" command followed by the platform name. This command compiles the application and generates executable files for the selected platform.

4. Run the project: To run the Cordova project on a device or emulator, the developer uses the "cordova run" command followed by the platform name. This command deploys the compiled application on the selected platform.

5. Plugin management: Plugins are used to add functionality to the Cordova project. The "cordova plugin" command is used to search, install, update, and remove plugins.

In summary, the "cordova" command is used for building, managing, and deploying hybrid mobile applications that serve as a bridge between web technologies and mobile devices. 

## tldr 
 
> Mobile apps with HTML, CSS & JS.
> More information: <https://cordova.apache.org/docs/en/latest/guide/cli/>.

- Create a Cordova project:

`cordova create {{path}} {{package_name}} {{project_name}}`

- Display the current workspace status:

`cordova info`

- Add a Cordova platform:

`cordova platform add {{platform}}`

- Remove a Cordova platform:

`cordova platform remove {{platform}}`

- Add a Cordova plugin:

`cordova plugin add {{pluginid}}`

- Remove a Cordova plugin:

`cordova plugin remove {{pluginid}}`
