# ldd 
## chatgpt 
`ldd` is a Linux command that is used to print the shared library dependencies of a binary executable or a dynamically linked shared object file. 

Here is the syntax for `ldd`:

```
ldd [option]... file...
```

- `option`: This is an optional parameter that can be used to change the behavior of the `ldd` command. One common option is `-d`, which enables the printing of indirect dependencies as well. 

- `file`: This is the name of the binary executable or shared object file whose shared library dependencies are to be displayed.

When the `ldd` command is executed with a given file name as an argument, it scans the file and generates a list of all the dynamic libraries required by that executable file or shared object file. These libraries are searched in the standard library directories as well as any user-defined directories specified by the `LD_LIBRARY_PATH` environment variable.

The output of the `ldd` command includes the name and path of the shared library dependencies, the libraries' version numbers, and their memory address locations in the system. If a library is missing, either because it is not installed or because it cannot be found, then `ldd` will indicate the missing dependency in its output.

The `ldd` command is useful in identifying potential issues with missing dependencies when trying to run an executable file or shared object file on a Linux system. It is also helpful in the debugging process when trying to resolve issues related to shared library dependencies. 

## tldr 
 
> Display shared library dependencies of a binary.
> Do not use on an untrusted binary, use objdump for that instead.
> More information: <https://manned.org/ldd>.

- Display shared library dependencies of a binary:

`ldd {{path/to/binary}}`

- Display all information about dependencies:

`ldd --verbose {{path/to/binary}}`

- Display unused direct dependencies:

`ldd --unused {{path/to/binary}}`

- Report missing data objects and perform data relocations:

`ldd --data-relocs {{path/to/binary}}`

- Report missing data objects and functions, and perform relocations for both:

`ldd --function-relocs {{path/to/binary}}`
