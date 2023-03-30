# pkg-config 
## chatgpt 
pkg-config is a command-line tool used to retrieve information regarding the installed libraries on a Unix/Linux system. This tool helps in making the process of building and compiling software easier by providing the necessary information required by the build system for a library. 

When invoked with the name of a library, pkg-config will return the version number, the compiler and linker flags needed to link against the library, and any dependencies required. This information can then be used to configure and build the software that uses the library.

The command syntax for pkg-config is as follows:

    $ pkg-config [options] [library_name]

Here, "[options]" are any command-line options that can be used with pkg-config, and "[library_name]" is the name of the library whose information is required.

Some of the frequently used options with pkg-config include:

- --cflags: Returns the flags required to compile code that uses the library.
- --libs: Returns the flags required to link against the library.
- --modversion: Returns the version number of the library.
- --atleast-version: Returns a boolean value indicating if the library version is at least the specified version.

Overall, pkg-config is an important tool for developers building software on Unix/Linux systems as it simplifies the process of retrieving library information required for building software. 

## tldr 
 
> Provide the details of installed libraries for compiling applications.
> More information: <https://www.freedesktop.org/wiki/Software/pkg-config/>.

- Get the list of libraries and their dependencies:

`pkg-config --libs {{library1 library2 ...}}`

- Get the list of libraries, their dependencies, and proper cflags for gcc:

`pkg-config --cflags --libs {{library1 library2 ...}}`

- Compile your code with libgtk-3, libwebkit2gtk-4.0 and all their dependencies:

`c++ example.cpp $(pkg-config --cflags --libs gtk+-3.0 webkit2gtk-4.0) -o example`
