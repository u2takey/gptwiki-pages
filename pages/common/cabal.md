# cabal 
## chatgpt 
Cabal is a command-line tool used for building, managing, and sharing Haskell libraries and applications. It is similar to other package managers like npm and pip.

Cabal commands are used to interact with packages and libraries in the Haskell ecosystem. Here are some common commands:

- init: Initializes a new Cabal project, creating a .cabal file and a src directory with a Main.hs file.
- build: Builds the project and generates executable files.
- install: Installs the project and its dependencies.
- update: Updates the list of available packages and dependencies.
- clean: Removes temporary files generated during the build process.
- info: Displays information about a package, including its version, dependencies, and description.
- list: Displays a list of installed packages and their versions.

Cabal also supports a number of flags and options that can be used with these commands. For example, the --lib flag can be used with the install command to install only the library portion of a package, rather than any executables or tests that may be included. The --only-dependencies flag can be used with the build command to only build the dependencies of a package, rather than the package itself.

In summary, Cabal is a powerful tool that helps Haskell developers manage dependencies and build robust applications. 

## tldr 
 
> Command-line interface to the Haskell package infrastructure (Cabal).
> Manage Haskell projects and Cabal packages from the Hackage package repository.
> More information: <https://cabal.readthedocs.io/en/latest/intro.html>.

- Search and list packages from Hackage:

`cabal list {{search_string}}`

- Show information about a package:

`cabal info {{package_name}}`

- Download and install a package:

`cabal install {{package_name}}`

- Create a new Haskell project in the current directory:

`cabal init`

- Build the project in the current directory:

`cabal build`

- Run tests of the project in the current directory:

`cabal test`
