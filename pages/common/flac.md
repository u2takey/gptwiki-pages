# flac 
## chatgpt 
The flac command is used to encode, decode, test and manipulate audio files in the FLAC (Free Lossless Audio Codec) format. It is a command-line utility that is available for Linux, Windows, and macOS.

The general syntax for the flac command is as follows:

flac [options] [filename]

Where [options] are the various command line options that can be specified for the flac command and [filename] is the name of the file that you want to encode/decode/test.

Here are some of the most common options that can be used with the flac command:

- -d: This option is used to decode a FLAC file. It will take a FLAC file as input and produce an uncompressed audio file as output (e.g. WAV).
- -e: This option is used to encode a WAV file to FLAC format.
- -c: This option is used to output the result to the console instead of a file.
- -t: This option is used to test a FLAC file for errors.
- -V: This option is used to specify the compression level (0-8), where 0 is uncompressed and 8 is the highest compression level.
- -b: This option is used to specify the block size.

In summary, the flac command is a versatile tool for working with FLAC audio files in a command-line environment. It can be used to encode, decode, test and manipulate audio files with ease, providing a range of options for customization and optimization. 

## tldr 
 
> Encodes, decodes and tests FLAC files.
> More information: <https://xiph.org/flac>.

- Encode a WAV file to FLAC (this will create a FLAC file in the same location as the WAV file):

`flac {{path/to/file.wav}}`

- Encode a WAV file to FLAC, specifying the output file:

`flac -o {{path/to/output.flac}} {{path/to/file.wav}}`

- Decode a FLAC file to WAV, specifying the output file:

`flac -d -o {{path/to/output.wav}} {{path/to/file.flac}}`

- Test a FLAC file for the correct encoding:

`flac -t {{path/to/file.flac}}`
