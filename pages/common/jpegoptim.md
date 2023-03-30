# jpegoptim 
## chatgpt 
jpegoptim is a command-line utility used to optimize JPEG images to reduce their file size without compromising the quality of the image. This tool is used to compress JPEG files by removing unnecessary data, such as comments and metadata, and by adjusting the quality level of the image to reduce the file size.

The command can be used in the following format:

jpegoptim [options] filename.jpg

Here are some common options that can be used with jpegoptim:

- -r, --recurse: Compress all JPEG files in the given directory and its subdirectories.

- -t, --threshold: Set the minimum percentage savings that must be achieved for an image to be optimized.

- -m, --max-quality: Specify the maximum quality level (1-100) for compression. By default, this is set to 85.

- -s, --strip: Strip all metadata and comments from the JPEG file.

- -d, --dest: Specify a destination directory for the compressed file.

Once the command is executed, the tool will optimize the JPEG file and save a copy of the compressed file in the specified destination directory, or in the same directory as the original file. The output file will have a smaller file size than the original, but will have the same quality level. 

## tldr 
 
> Optimise JPEG images.
> More information: <https://github.com/tjko/jpegoptim>.

- Optimise a set of JPEG images, retaining all associated data:

`jpegoptim {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}`

- Optimise JPEG images, stripping all non-essential data:

`jpegoptim --strip-all {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}`

- Force the output images to be progressive:

`jpegoptim --all-progressive {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}`

- Force the output images to have a fixed maximum filesize:

`jpegoptim --size={{250k}} {{image1.jpeg}} {{image2.jpeg}} {{imageN.jpeg}}`
