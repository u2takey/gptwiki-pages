# flutter 
## chatgpt 
Flutter is a command-line tool that is used for developing mobile applications for Android and iOS. It is an open-source tool that enables developers to create visually appealing and high-performing applications by using a single codebase.

When you run the "flutter" command in your terminal, the tool initializes and provides you with a set of subcommands that can be used for various tasks such as creating a new Flutter project, running an existing project, and managing packages used in the project. The subcommands that can be used with the flutter command include:

1. create - This subcommand is used to create a new Flutter project. It creates a new directory with the project structure and files.

2. run - This subcommand is used to run an existing Flutter project on an emulator, simulator, or physical device. It also provides options to run the app in release mode or debug mode.

3. build - This subcommand is used to build an apk or ipa file for the Flutter application. It provides options to build the application for a specific platform (Android or iOS), in debug or release mode, and with other platform-specific configurations.

4. doctor - This subcommand is used to check if the Flutter environment is set up correctly and provides information about any missing dependencies or issues that need to be resolved.

5. packages - This subcommand is used to manage the packages used in the Flutter project. It enables developers to add, remove, or update packages from the project.

Overall, the flutter command is the starting point for creating and managing Flutter projects, and it provides a range of subcommands that simplify development tasks and enhance the developer experience. 

## tldr 
 
> Google's free, open source, and cross-platform mobile app SDK.
> More information: <https://github.com/flutter/flutter/wiki/The-flutter-tool>.

- Initialize a new Flutter project in a directory of the same name:

`flutter create {{project_name}}`

- Check if all external tools are correctly installed:

`flutter doctor`

- List or change Flutter channel:

`flutter channel {{stable|beta|dev|master}}`

- Run Flutter on all started emulators and connected devices:

`flutter run -d all`

- Download all packages specified in `pubspec.yaml`:

`flutter pub get`

- Run tests in a terminal from the root of the project:

`flutter test {{test/example_test.dart}}`

- Build a release APK targeting most modern smartphones:

`flutter build apk --target-platform {{android-arm}},{{android-arm64}}`

- Display help about a specific command:

`flutter help {{command}}`
