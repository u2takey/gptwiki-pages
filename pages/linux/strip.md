# strip 
## chatgpt 
The "strip" command is used in Linux and Unix based systems to remove symbols and debugging information from binary files. It can also be used to reduce the size of the binary file by removing unnecessary information. This command is commonly used by developers to produce smaller and efficient binary files for distribution.

Some of the common options used with the "strip" command are:

1. "-s" - This option is used to strip symbol table information from the binary file.

2. "-g" - This option is used to strip debugging information from the binary file.

3. "-o" - This option is used to specify the output file name.

4. "-p" - This option is used to preserve the file time and mode.

5. "-R" - This option is used to remove a specific symbol or section from the binary file.

For Example, the command: "strip -s -o output_file input_file" will create a new file called "output_file" which contains the stripped version of the binary file "input_file" by removing the symbol table information. 

## tldr 
 
> Discard symbols from executables or object files.
> More information: <https://manned.org/strip>.

- Replace the input file with its stripped version:

`strip {{path/to/file}}`

- Strip symbols from a file, saving the output to a specific file:

`strip {{path/to/input_file}} -o {{path/to/output_file}}`

- Strip debug symbols only:

`strip --strip-debug {{path/to/file.o}}`
