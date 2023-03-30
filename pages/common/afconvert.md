# afconvert 
## chatgpt 
`afconvert` is a command-line tool on macOS that lets you convert audio files from one format to another. The `afconvert` command can be used to perform various operations on audio files. Here are the details:

Syntax:
```
afconvert [options] input_file [output_file]
```

Options:
- `-h`: Display help information, including a list of supported audio file formats.
- `-f format`: Specify the output audio file format. For example, `-f mp3` or `-f aac`.
- `-d codec`: Specify the output audio codec. For example, `-d LEI16@44100` or `-d alac`.
- `-b bitrate`: Specify the output bitrate in bits per second.
- `-c channels`: Specify the number of output channels (1 for mono, 2 for stereo).
- `-s sample_rate`: Specify the output sample rate in Hz.
- `-q quality`: Specify the output quality level (0-127, with 127 being the highest quality).
- `-t time`: Specify a duration for the output file in seconds.

Usage:
```
afconvert input_file.aiff -f mp3 output_file.mp3
```
The above command will convert the input_file.aiff file to MP3 format and save it as output_file.mp3.

Note:
`afconvert` can be used to convert many different file formats, including AIFF, WAV, MP3, AAC, Apple Lossless, and more. The tool can also be used to perform sample rate and channel conversions, apply effects, and do other audio processing tasks. 

## tldr 
 
> Convert between AFF and raw file formats.
> More information: <https://manned.org/afconvert.1>.

- Use a specific extension (default: `aff`):

`afconvert -a {{extension}} {{path/to/input_file}} {{path/to/output_file1 path/to/output_file2 ...}}`

- Use a specific compression level (default: `7`):

`afconvert -X{{0..7}} {{path/to/input_file}} {{path/to/output_file1 path/to/output_file2 ...}}`
