# react-native 
## chatgpt 
React Native is a framework used for building native mobile applications using JavaScript and React.

The command "react-native" is used to interact with the React Native CLI (Command Line Interface) tool. It allows developers to create, start, and manage new React Native projects; run and debug applications on the Android and iOS devices or emulators; and perform various development tasks, such as bundling, building, and testing the app.

Here are some of the sub-commands and their functions:

- init: Initializes a new React Native project.
- start: Starts the development server and the app on an emulator or device.
- run-android: Builds and runs the app on an Android device or emulator.
- run-ios: Builds and runs the app on an iOS device or emulator.
- test: Runs the tests in the project using Jest.
- bundle: Bundles the app code into a single file.

Using the "react-native" command, developers can create, develop, and deploy mobile applications using React Native. 

## tldr 
 
> A framework for building native apps with React.
> More information: <https://reactnative.dev>.

- Initialize a new React Native project in a directory of the same name:

`react-native init {{project_name}}`

- Start the metro bundler:

`react-native start`

- Start the metro bundler with a clean cache:

`react-native start --reset-cache`

- Build the current application and start it on a connected Android device or emulator:

`react-native run-android`

- Build the current application and start it on an iOS simulator:

`react-native run-ios`

- Build the current application in `release` mode and start it on a connected Android device or emulator:

`react-native run-android --variant={{release}}`

- Start `logkitty` and print logs to `stdout`:

`react-native log-android`

- Start `tail system.log` for an iOS simulator and print logs to `stdout`:

`react-native log-ios`
