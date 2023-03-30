# base32 
## chatgpt 
Base32 is a command that is used to encode and decode data using the Base32 encoding scheme. Base32 encoding is a way of representing binary data using a sequence of 32 characters that are easier to transmit over networks or store in text-based formats.

The Base32 encoding scheme uses a set of 32 characters, which include the letters A-Z (excluding I, L, and O) and digits 2-7. These characters are used to represent the 32 possible values of a 5-bit binary number.

The syntax for using the Base32 command may vary depending on the implementation, but it generally follows the format:

base32 [options] [filename]

To encode a file using Base32, you can use the following command:

$ base32 input_file > output_file

This command will read the contents of the input file and convert it into Base32 format, which will then be written to the output file.

To decode a Base32-encoded file, use the following command:

$ base32 -d input_file > output_file

This command will read the Base32-encoded input file and convert it back into the original binary format, which will then be written to the output file.

Some common options that can be used with the Base32 command include:

-d: decode the input file
-w [number]: wrap lines at the specified number of characters (default is 76) 

## tldr 
 
> Encode or decode file or standard input to/from Base32, to standard output.
> More information: <https://www.gnu.org/software/coreutils/base32>.

- Encode a file:

`base32 {{path/to/file}}`

- Decode a file:

`base32 --decode {{path/to/file}}`

- Encode from `stdin`:

`{{somecommand}} | base32`

- Decode from `stdin`:

`{{somecommand}} | base32 --decode`
