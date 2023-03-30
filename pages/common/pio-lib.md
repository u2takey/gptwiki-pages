# pio lib 
## chatgpt 
pio lib is a Command Line Interface (CLI) command for interacting with the libraries feature of the PlatformIO ecosystem. 

The "lib" part in the command stands for "library". PlatformIO libraries are collections of code that offer functionalities to your projects. They can contain source codes, header files, examples, documentation, licenses, configuration files, etc.

When you use the "pio lib" command, you can do several things like:

1. Search for libraries in the PlatformIO Registry:
You can use "pio lib search" command followed by a keyword to find libraries available in the PlatformIO Registry. When you see the right library, you can use "pio lib install" to install it to your project.

2. Install a library:
You can use "pio lib install" followed by the library's name and version to install it directly to your project. PlatformIO will download the library from the registry and add it to your project.

3. List installed libraries:
You can use "pio lib list" to see a list of all the libraries that you have installed in the current project.

4. Update a library:
You can use "pio lib update" followed by the library's name to update it to the latest version available in the registry.

Overall, the "pio lib" command is a powerful feature of the PlatformIO ecosystem that allows you to easily add, manage and update libraries for your projects. 

## tldr 
 
> Manage PlatformIO libraries.
> More information: <https://docs.platformio.org/en/latest/core/userguide/lib/>.

- List installed libraries:

`pio lib list`

- List built-in libraries based on installed development platforms and their frameworks:

`pio lib builtin`

- Search for existing libraries:

`pio lib search {{keyword}}`

- Show details about a library:

`pio lib show {{library}}`

- Install a library:

`pio lib install {{library}}`

- Update installed libraries:

`pio lib update`

- Uninstall a library:

`pio lib uninstall {{library}}`

- Show PlatformIO library registry statistics:

`pio lib stats`
