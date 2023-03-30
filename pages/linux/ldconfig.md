# ldconfig 
## chatgpt 
ldconfig is a command-line tool used in Unix and Linux systems to configure dynamic linker runtime bindings. It maintains the runtime library cache, which lists the shared libraries installed on the system and their locations. When an application is run, the dynamic linker reads this cache to determine the location of the required shared libraries.

The ldconfig command can be used to update the runtime library cache. When new shared libraries are installed on the system, the ldconfig command must be run to update the cache with the new library information. The command scans directories specified in the "/etc/ld.so.conf" file, as well as the "/usr/lib" and "/lib" directories, and adds any new libraries to the cache.

The syntax for the ldconfig command is as follows:

ldconfig [options] [directory]

The options available for ldconfig include:

- -n: Perform a dry run and do not modify the runtime library cache
- -f file: Use the specified cache file instead of the default "/etc/ld.so.cache"
- -v: Enable verbose mode and display debugging information
- -X: Disable cache generation and display the library dependencies for the specified file

The directory parameter specifies a directory where ldconfig should look for shared libraries, in addition to the directories listed in the "/etc/ld.so.conf" file. Multiple directories can be specified by separating them with a colon.

Overall, the ldconfig command ensures that the runtime linker can find and load the required shared libraries for a given application, enhancing the performance and reliability of the system. 

## tldr 
 
> Configure symlinks and cache for shared library dependencies.
> More information: <https://manned.org/ldconfig>.

- Update symlinks and rebuild the cache (usually run when a new library is installed):

`sudo ldconfig`

- Update the symlinks for a given directory:

`sudo ldconfig -n {{path/to/directory}}`

- Print the libraries in the cache and check whether a given library is present:

`ldconfig -p | grep {{library_name}}`
