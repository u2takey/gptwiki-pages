# ufraw-batch 
## chatgpt 
The `ufraw-batch` command is a command-line tool used to convert RAW image files to other file formats, such as JPEG or TIFF. The tool is a part of the UFRaw software package, which is designed specifically for working with RAW image files.

The command syntax for `ufraw-batch` is as follows:

`ufraw-batch [options] input_file [output_file]`

Here's what each part of the command means:

- `ufraw-batch`: This is the name of the command.
- `[options]`: These are optional arguments that can be passed to the command to modify its behavior. Examples of options include setting brightness, contrast, and saturation levels for the output image.
- `input_file`: This is the name of the RAW image file you want to convert.
- `[output_file]`: This is the name of the file that will be created when the RAW image file is converted. If no output file is specified, the tool will create a file with the same name as the input file, but with a different file extension.

To use `ufraw-batch`, simply open up a command prompt or terminal window, navigate to the directory where the RAW image files are stored, and enter the appropriate command with the necessary options and file names. The tool will then begin converting the RAW image file to the specified output format. 

## tldr 
 
> Convert RAW files from cameras into standard image files.
> More information: <https://manned.org/ufraw-batch>.

- Simply convert RAW files to JPG:

`ufraw-batch --out-type=jpg {{input_file(s)}}`

- Simply convert RAW files to PNG:

`ufraw-batch --out-type=png {{input_file(s)}}`

- Extract the preview image from the raw file:

`ufraw-batch --embedded-image {{input_file(s)}}`

- Save the file with size up to the given maximums MAX1 and MAX2:

`ufraw-batch --size=MAX1,MAX2 {{input_file(s)}}`
