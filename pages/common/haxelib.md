# haxelib 
## chatgpt 
haxelib is a command-line tool used in Haxe programming language that allows developers to manage, install and upgrade packages and libraries for Haxe projects. 

Here is a brief description of various sub-commands for haxelib:

1. install - It is used to install a specific library or package from the Haxe repository. The command format is haxelib install library-name.

2. list - This command is used to list all the libraries installed on the system or a specific library's details.

3. upgrade - It is used to upgrade a specific library or all the libraries installed on the system. The command format is haxelib upgrade library-name.

4. remove - This command is used to remove a specific library or all the libraries installed on the system. The command format is haxelib remove library-name.

5. search - It is used to search for a specific library or all the available libraries in the Haxe repository. The command format is haxelib search library-name.

6. openfl - It is used to create or manage OpenFL projects. 

Overall, haxelib is an essential tool for managing dependencies in Haxe projects. It makes the process of installing, removing, upgrading, and searching for libraries more comfortable and efficient for developers. 

## tldr 
 
> Haxe Library Manager.
> More information: <https://lib.haxe.org/>.

- Search for a Haxe library:

`haxelib search {{keyword}}`

- Install a Haxe library:

`haxelib install {{libname}}`

- Install a specific version of a Haxe library:

`haxelib install {{libname}} {{version}}`

- Upgrade all installed Haxe libraries:

`haxelib upgrade`

- Install the development version of a library from a Git repository:

`haxelib git {{libname}} {{git_url}}`

- Uninstall a Haxe library:

`haxelib remove {{libname}}`

- Print a tree of locally installed Haxe libraries:

`haxelib list`
