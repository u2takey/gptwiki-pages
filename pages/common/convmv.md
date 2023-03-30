# convmv 
## chatgpt 
`convmv` is a Linux command that converts the encoding of filenames and the content of files. It can convert between different character sets like UTF-8, ISO-8859, or different national encodings. It preserves the file attributes like ownership or permissions and can operate recursively on an entire directory structure.

Here is the basic syntax for the `convmv` command:

```
convmv [options] -f encoding -t encoding [--notest] file/directory
```

The options that are available with `convmv` are:

- `-f` or `--from-code`: Specify the encoding of the source files. For example, `-f ISO-8859-1` specifies the ISO-8859-1 character set.
- `-t` or `--to-code`: Specify the target encoding for conversion. For example, `-t UTF-8` specifies the UTF-8 character set.
- `-r` or `--recursive`: Convert the files in the directory and any subdirectories recursively.
- `-i` or `--interactive`: Prompts before overwriting existing files.
- `--notest`: Perform the conversion without making any changes. This option is useful for checking the results of the conversion before actually applying it to the files.

Here's an example command that converts the encoding of all files in the current directory from iso-8859-1 to utf-8:

```
convmv -f iso-8859-1 -t utf-8 -r .
```

In this example, the `-r` option is used to convert the files recursively in the current directory and any subdirectories. The `.` at the end specifies the target directory as the current directory.

Overall, `convmv` is a flexible command-line utility that can be used to convert the character encoding of filenames and file content in a Linux environment. 

## tldr 
 
> Convert filenames (NOT file content) from one encoding to another.
> More information: <https://www.j3e.de/linux/convmv/man/>.

- Test filename encoding conversion (don't actually change the filename):

`convmv -f {{from_encoding}} -t {{to_encoding}} {{input_file}}`

- Convert filename encoding and rename the file to the new encoding:

`convmv -f {{from_encoding}} -t {{to_encoding}} --notest {{input_file}}`
