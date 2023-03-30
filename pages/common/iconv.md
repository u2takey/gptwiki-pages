# iconv 
## chatgpt 
The iconv command is a utility program that converts between different character sets or encodings. 

Syntax: 

```
iconv [OPTION...] [-f ENCODING] [-t ENCODING] [INPUTFILE]
```

Options:

- `-f ENCODING`: specifies the input encoding, which is the character set of the input file.
- `-t ENCODING`: specifies the target encoding, which is the character set to which the input file will be converted.
- `-c`: ignores invalid characters in the input file.
- `-o`: specifies the output file name.
- `-l`: lists all available encodings on the system.

Example:

1. Convert a file from UTF-8 to ASCII encoding:

```
iconv -f UTF-8 -t ASCII input.txt > output.txt
```

In this command, the input file `input.txt` is in the UTF-8 encoding, and we want to convert it to ASCII encoding. The `>` character is used to redirect the output to a file named `output.txt`.

2. Ignore invalid characters during conversion:

```
iconv -f UTF-8 -t ASCII//IGNORE input.txt
```

In this command, the `//IGNORE` option is used to tell iconv to ignore invalid characters in the input file.

3. List all available encodings:

```
iconv -l
```

This command lists all available character sets and encodings supported by the system. 

## tldr 
 
> Converts text from one encoding to another.
> More information: <https://manned.org/iconv>.

- Convert file to a specific encoding, and print to `stdout`:

`iconv -f {{from_encoding}} -t {{to_encoding}} {{input_file}}`

- Convert file to the current locale's encoding, and output to a file:

`iconv -f {{from_encoding}} {{input_file}} > {{output_file}}`

- List supported encodings:

`iconv -l`
