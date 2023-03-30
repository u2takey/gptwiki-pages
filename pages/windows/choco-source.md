# choco source 
## chatgpt 
The "choco source" command is a command-line interface tool that is used to manage the Chocolatey package source configuration. It allows the user to add, remove, and modify package sources. 

Package sources are essentially locations where Chocolatey can download software packages. By default, Chocolatey uses the official package source called the Chocolatey Community Repository (CCR). However, users can add additional sources to Chocolatey, such as private repositories or other community repositories, to access more software packages.

When the "choco source" command is executed, it displays a list of all configured package sources. It gives details about each source such as the name, URL, username, password, and priority assigned to each source. The user can modify and remove existing package sources, as well as add new ones, specifying the required information like name, URL, and other credentials, to configure Chocolatey to connect to their required source.

In summary, the "choco source" command is a tool that helps in managing the configuration of package sources for Chocolatey package manager, which makes it easier for users to access and install a wide variety of software packages available from various sources. 

## tldr 
 
> Manage sources for packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-source>.

- List currently available sources:

`choco source list`

- Add a new package source:

`choco source add --name {{name}} --source {{url}}`

- Add a new package source with credentials:

`choco source add --name {{name}} --source {{url}} --user {{username}} --password {{password}}`

- Add a new package source with a client certificate:

`choco source add --name {{name}} --source {{url}} --cert {{path\to\certificate_file}}`

- Enable a package source:

`choco source enable --name {{name}}`

- Disable a package source:

`choco source disable --name {{name}}`

- Remove a package source:

`choco source remove --name {{name}}`
