# base64 
## chatgpt 
The base64 command is a utility in Unix/Linux systems that encodes data in base64 format or decodes data from base64 format. The base64 utility is used to transform binary data into a printable ASCII format, which is useful for transmitting data over networks that cannot handle non-printable characters.

The base64 command typically takes the following form:

```
base64 [option]... [file]
```

The options that can be used with the base64 command include:

- `-d` or `--decode`: decode the input from base64 format instead of encoding it
- `-i` or `--ignore-garbage`: ignore non-base64 characters in the input stream
- `-w [number]` or `--wrap-around=[number]`: wrap encoded lines after `number` characters (defaults to 76)

The `[file]` argument is optional and specifies the input file to encode or decode. If no `[file]` argument is provided, the command reads from standard input.

Some examples of using the base64 command are:

```
# A simple encoding example
$ echo "hello world" | base64
aGVsbG8gd29ybGQK

# A decoding example
$ echo "aGVsbG8gd29ybGQK" | base64 -d
hello world
```

In the above example, the text "hello world" is encoded using base64 and then decoded back to its original form using the `-d` option. 

## tldr 
 
> Encode or decode file or standard input to/from Base64, to standard output.
> More information: <https://www.gnu.org/software/coreutils/base64>.

- Encode the contents of a file as base64 and write the result to `stdout`:

`base64 {{path/to/file}}`

- Decode the base64 contents of a file and write the result to `stdout`:

`base64 --decode {{path/to/file}}`

- Encode from `stdin`:

`{{somecommand}} | base64`

- Decode from `stdin`:

`{{somecommand}} | base64 --decode`
