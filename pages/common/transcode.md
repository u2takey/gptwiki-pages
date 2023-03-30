# transcode 
## chatgpt 
The command "transcode" is used to convert multimedia files from one format to another. This command is used in the Linux operating system.

When you use the "transcode" command, you need to pass various options and parameters to specify the input and output files, codecs, filters, and other settings.

Here are some common options used with the "transcode" command:

- -i: Specifies the input file name
- -o: Specifies the output file name
- -x: Specifies various settings, such as the codec, resolution, and bitrate
- -y: Specifies filters, such as cropping, scaling, and deinterlacing
- -S: Enables parallel processing to speed up the conversion process

Here's an example of using the "transcode" command to convert an MPEG-2 file to H.264 format:

transcode -i input.mpg -x mpeg2,h264 -o output.mp4

In this example, we specify the input file using the "-i" option and the output file using the "-o" option. We also specify the codecs to use for input and output using the "-x" option (mpeg2 for input and h264 for output).

The "transcode" command is a powerful tool that can be used for various multimedia conversion tasks. However, it's important to have a basic understanding of codecs, filters, and other settings before using this command to avoid unexpected results. 

## tldr 
 
> Transcode video and audio codecs, and convert between media formats.
> More information: <https://manned.org/transcode>.

- Create stabilization file to be able to remove camera shakes:

`transcode -J stabilize -i {{input_file}}`

- Remove camera shakes after creating stabilization file, transform video using XviD:

`transcode -J transform -i {{input_file}} -y xvid -o {{output_file}}`

- Resize the video to 640x480 pixels and convert to MPEG4 codec using XviD:

`transcode -Z 640x480 -i {{input_file}} -y xvid -o {{output_file}}`
