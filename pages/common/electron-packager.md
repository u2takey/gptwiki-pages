# electron-packager 
## chatgpt 
Electron-packager is a command-line tool for building native desktop apps using Electron, a framework for building cross-platform desktop apps using web technologies such as HTML, CSS, and JavaScript.

The electron-packager command is used to package an Electron app into executable files for different operating systems such as Windows, macOS, and Linux. This command takes a number of parameters, including the path to the app's source code, the name of the app, and the target operating system and architecture. 

The basic syntax for the electron-packager command is:

```
electron-packager <sourcedir> <appname> [options]
```

Where:
 - `<sourcedir>` is the path to the directory containing the app's source code
 - `<appname>` is the name of the app
 - `[options]` are additional settings that can be used to fine-tune the packaging process, such as target platform, architecture, icons, and version number.

By default, electron-packager will create a directory containing executable files for the specified platform and architecture. These files can then be distributed to users as standalone desktop apps. 

Overall, the electron-packager command is an important tool for building, packaging, and distributing native desktop apps created using Electron. 

## tldr 
 
> A tool used to build Electron app executables for Windows, Linux and macOS.
> Requires a valid package.json in the application directory.
> More information: <https://github.com/electron/electron-packager>.

- Package an application for the current architecture and platform:

`electron-packager "{{path/to/app}}" "{{app_name}}"`

- Package an application for all architectures and platforms:

`electron-packager "{{path/to/app}}" "{{app_name}}" --all`

- Package an application for 64-bit Linux:

`electron-packager "{{path/to/app}}" "{{app_name}}" --platform="{{linux}}" --arch="{{x64}}"`

- Package an application for ARM macOS:

`electron-packager "{{path/to/app}}" "{{app_name}}" --platform="{{darwin}}" --arch="{{arm64}}"`
