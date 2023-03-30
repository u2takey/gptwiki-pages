# file 
## chatgpt 
The `file` command is a Linux/Unix utility that is used to determine the type of a given file. When you execute the `file` command followed by the name of a file as an argument, it reads information from the file's contents and presents the file type information to you.

The output of the `file` command includes various details about the specified file, such as the file's format, encoding, file type, and other important information. It can help you quickly determine whether a file is a text file, binary file, image file, compressed file, or any other type of file.

Here's an example of how the `file` command works:

```
$ file myfile.txt
myfile.txt: ASCII text
```

In this example, the `file` command tells us that `myfile.txt` is an ASCII text file. It can be used to determine the file type of any file on your system, and is especially useful when working with unknown or corrupted files. 

## tldr 
 
> Determine file type.
> More information: <https://manned.org/file>.

- Give a description of the type of the specified file. Works fine for files with no file extension:

`file {{path/to/file}}`

- Look inside a zipped file and determine the file type(s) inside:

`file -z {{foo.zip}}`

- Allow file to work with special or device files:

`file -s {{path/to/file}}`

- Don't stop at first file type match; keep going until the end of the file:

`file -k {{path/to/file}}`

- Determine the MIME encoding type of a file:

`file -i {{path/to/file}}`
