# qrencode 
## chatgpt 
qrencode is a command line utility that creates QR codes from text or data input, allowing you to encode information into a scannable matrix barcode. The command works by taking input from either a file or standard input, and outputs the resulting QR code image to the console, a file, or a printer.

The general syntax of the qrencode command is as follows: 

`qrencode [options] [text/data]`

Where `[options]` are additional parameters that can be passed to the command, such as the encoding type, error correction level, and output image format. `[text/data]` refers to the input that is to be encoded into the QR code.

Some common options for the qrencode command include:

- `-s`: Set the size of the QR code (default is 3)
- `-l`: Set the error correction level (L, M, Q, or H)
- `-o`: Set the output file for the generated image
- `-t`: Set the output terminal for the generated image (e.g. stdout, ansi, utf8)
- `-i`: Interpret the input as binary data instead of text

For example, to create a QR code for the text "Hello World" with a size of 5 and high error correction level, you could use the following command:

`qrencode -s 5 -l H "Hello World"`

The resulting QR code image would be displayed in the console output. Alternatively, you could output the image to a file by adding the `-o` option:

`qrencode -s 5 -l H -o hello_world.png "Hello World"`

This would create a PNG image file named `hello_world.png` in the current directory containing the generated QR code. 

## tldr 
 
> QR Code generator. Supports PNG and EPS.
> More information: <https://fukuchi.org/works/qrencode>.

- Convert a string to a QR code and save to an output file:

`qrencode -o {{path/to/output_file.png}} {{string}}`

- Convert an input file to a QR code and save to an output file:

`qrencode -o {{path/to/output_file.png}} -r {{path/to/input_file}}`

- Convert a string to a QR code and print it in terminal:

`qrencode -t ansiutf8 {{string}}`

- Convert input from pipe to a QR code and print it in terminal:

`echo {{string}} | qrencode -t ansiutf8`
