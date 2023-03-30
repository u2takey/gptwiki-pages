# readelf 
## chatgpt 
`readelf` is a command-line utility tool that reads and displays information from object files, such as executables, shared libraries, and object files. It is typically used in the context of debugging and analysis of binary files.

The basic syntax of the `readelf` command is as follows:

```
readelf [options] file
```

where `file` is the name of the object file to be inspected and `[options]` are command line options used to control the output and behavior of `readelf`.

Some of the most common options used with `readelf` include:

- `-h` : Displays the header information of the ELF file.
- `-S` : Displays the section headers of the ELF file.
- `-s` : Displays the symbol table of the ELF file.
- `-r` : Displays the relocation table of the ELF file.
- `-d` : Displays the dynamic section of the ELF file.
- `-A` : Displays all of the above information.

The `readelf` command provides a lot of flexibility and can be used to extract a wealth of information from object files. For example, using the `-a` option, it can display all available information about the file, including its architecture, type, and section-specific details such as sizes, offsets and flags.

Overall, `readelf` is a powerful tool for understanding the inner workings of ELF binary files and is widely used by developers, security researchers, and system administrators. 

## tldr 
 
> Displays information about ELF files.
> More information: <http://man7.org/linux/man-pages/man1/readelf.1.html>.

- Display all information about the ELF file:

`readelf -all {{path/to/binary}}`

- Display all the headers present in the ELF file:

`readelf --headers {{path/to/binary}}`

- Display the entries in symbol table section of the ELF file, if it has one:

`readelf --symbols {{path/to/binary}}`

- Display the information contained in the ELF header at the start of the file:

`readelf --file-header {{path/to/binary}}`
