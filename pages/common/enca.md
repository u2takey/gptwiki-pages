# enca 
## chatgpt 
enca is a command-line tool used for detecting and converting the character encoding of a text file. It stands for Encoding CHAos detector.

Syntax: enca [options] [file]

Options:
- -L, --list            : List all available encodings supported by enca.
- -d, --diagnose        : Print the detected encoding of the file.
- -g, --guess           : Guess the encoding of the file.
- -c, --convert-to      : Specify the encoding to which the file should be converted.
- -f, --force-output    : Force output to be in a specific character encoding.
- -i, --input-charset   : Specify the character encoding of the input file.
- -o, --output-charset  : Specify the character encoding of the output file.
- -w, --overwrite       : Overwrite the original file.

The enca command can be used to identify the character encoding of a file by analyzing its contents. It can also help to convert a file from one encoding to another. For instance, if you have a file encoded in Cyrillic, but you want to convert it to UTF-8, enca can help you achieve this task. 

To detect the character encoding of a file, you can run the following command:
enca -d <filename>

To convert a file from one encoding to another, for instance, to convert a GB2312-encoded file to UTF-8, use the following command:
enca -L zh_CN -x UTF-8 -c GB2312 <filename>

This will convert the file from GB2312 encoding to UTF-8 encoding. 

In summary, enca is a powerful tool used for identifying and converting the character encoding of text files. 

## tldr 
 
> Detect and convert the encoding of text files.
> More information: <https://github.com/nijel/enca>.

- Detect file(s) encoding according to the system's locale:

`enca {{path/to/file1 path/to/file2 ...}}`

- Detect file(s) encoding specifying a language in the POSIX/C locale format (e.g. zh_CN, en_US):

`enca -L {{language}} {{path/to/file1 path/to/file2 ...}}`

- Convert file(s) to a specific encoding:

`enca -L {{language}} -x {{to_encoding}} {{path/to/file1 path/to/file2 ...}}`

- Create a copy of an existing file using a different encoding:

`enca -L {{language}} -x {{to_encoding}} < {{original_file}} > {{new_file}}`
