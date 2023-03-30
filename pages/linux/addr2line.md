# addr2line 
## chatgpt 
addr2line is a command-line tool that is used to convert addresses into file names and line numbers. It is primarily used in the context of debugging programs and libraries.

The command has several options and usage variations, but the basic syntax is as follows:

addr2line [-f] [-e executable] [address1] [address2] ...

Here, the options are:

- -f: This option prints the function name in addition to the file name and line number.
- -e: This option specifies the path to the executable that contains the addresses to be translated.

And the arguments are:

- address1, address2, etc.: These are the addresses to be translated. They can be in any format that the program being debugged uses, such as hexadecimal or decimal.

When the command is run, it reads the addresses and looks up their corresponding file names and line numbers in the debug symbols of the executable. If the -f option is used, it also prints the name of the function that contains the address.

The output of the command is in the format "filename:line_number" or "filename:function_name:line_number", depending on whether the -f option is used. If an address cannot be resolved, addr2line prints "???".

Overall, addr2line is a useful tool for developers who need to debug programs and libraries at the machine code level. 

## tldr 
 
> Convert addresses of a binary into file names and line numbers.
> More information: <https://manned.org/addr2line>.

- Display the filename and line number of the source code from an instruction address of an executable:

`addr2line --exe={{path/to/executable}} {{address}}`

- Display the function name, filename and line number:

`addr2line --exe={{path/to/executable}} --functions {{address}}`

- Demangle the function name for C++ code:

`addr2line --exe={{path/to/executable}} --functions --demangle {{address}}`
