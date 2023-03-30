# xxd 
## chatgpt 
The `xxd` command is a tool used in Unix and Unix-like operating systems for converting binary data to hexadecimal format and displaying it in various ways.

The basic syntax of the `xxd` command is:

```
xxd [options] [infile] [outfile]
```

Here are some of the commonly used options:

- `-b`: Displays the binary representation of each byte.
- `-c cols`: Specifies the number of columns per line.
- `-g bytes`: Specifies the number of bytes grouped together.
- `-l len`: Specifies the number of bytes to read from the input file.
- `-u`: Displays the hexadecimal output in uppercase.
- `-r`: Reverses the operation, converting hexadecimal back to binary.

The `xxd` command is often used to analyze binary files, such as executables and libraries, as well as binary data stored in files or transmitted over a network. It can be particularly useful for debugging and reverse engineering applications that require low-level analysis of data. 

## tldr 
 
> Create a hexadecimal representation (hexdump) from a binary file, or vice-versa.
> More information: <https://manned.org/xxd>.

- Generate a hexdump from a binary file and display the output:

`xxd {{input_file}}`

- Generate a hexdump from a binary file and save it as a text file:

`xxd {{input_file}} {{output_file}}`

- Display a more compact output, replacing consecutive zeros (if any) with a star:

`xxd -a {{input_file}}`

- Display the output with 10 columns of one octet (byte) each:

`xxd -c {{10}} {{input_file}}`

- Display output only up to a length of 32 bytes:

`xxd -l {{32}} {{input_file}}`

- Display the output in plain mode, without any gaps between the columns:

`xxd -p {{input_file}}`

- Revert a plaintext hexdump back into binary, and save it as a binary file:

`xxd -r -p {{input_file}} {{output_file}}`
