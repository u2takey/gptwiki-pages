# od 
## chatgpt 
The `od` command is a Unix system utility used to display the contents of binary files in octal, decimal, hexadecimal, and ASCII formats. It stands for "octal dump".

The basic syntax of the `od` command is as follows:

```
od [options] [filename]
```

Here, `filename` is the path to the binary file you want to examine. If `filename` is not specified, `od` will read from standard input.

Some of the commonly used options for `od` are:

- `-A`: Specify the output format. The available formats are `a` for ASCII, `c` for UTF-8, `d` for decimal, `o` for octal, `x` for hexadecimal, and `n` for no output.
- `-t`: Specify the type of input data. The available types are `a` for ASCII, `c` for characters, `d` for decimal, `f` for floating point numbers, `h` for 16-bit integers, `i` for 32-bit integers, `l` for 64-bit integers, `o` for octal, and `x` for hexadecimal.
- `-j`: Specify the byte offset at which to start reading the input file.
- `-N`: Specify the number of bytes to read from the input file.
- `-v`: Output pairs of ASCII characters as a single character instead of as two separate characters.
- `-w`: Specify the number of bytes to group together in the output.

Examples:

1. To display the contents of a file in hexadecimal format, run:
```
od -x file.bin
```

2. To display the first 10 bytes of a file in octal format, run:
```
od -N 10 -t o file.bin
```

3. To display the ASCII characters in a file and group them by 4 bytes, run:
```
od -t c -w4 file.bin
```

Overall, `od` is a useful tool for examining binary files and understanding their contents in various formats. 

## tldr 
 
> Display file contents in octal, decimal or hexadecimal format.
> Optionally display the byte offsets and/or printable representation for each line.
> More information: <https://www.gnu.org/software/coreutils/od>.

- Display file using default settings: octal format, 8 bytes per line, byte offsets in octal, and duplicate lines replaced with `*`:

`od {{path/to/file}}`

- Display file in verbose mode, i.e. without replacing duplicate lines with `*`:

`od -v {{path/to/file}}`

- Display file in hexadecimal format (2-byte units), with byte offsets in decimal format:

`od --format={{x}} --address-radix={{d}} -v {{path/to/file}}`

- Display file in hexadecimal format (1-byte units), and 4 bytes per line:

`od --format={{x1}} --width={{4}} -v {{path/to/file}}`

- Display file in hexadecimal format along with its character representation, and do not print byte offsets:

`od --format={{xz}} --address-radix={{n}} -v {{path/to/file}}`

- Read only 100 bytes of a file starting from the 500th byte:

`od --read-bytes {{100}} --skip-bytes={{500}} -v {{path/to/file}}`
