# identify 
## chatgpt 
The `identify` command is a utility command that is used to identify an image's properties and metadata. 

When used with an image as an argument, the identify command displays the following information about the image:

- The image file name and format (jpeg, png, gif, etc.)
- The image size (width x height)
- The number of pixels and the aspect ratio
- The color profile and depth
- The image resolution (in DPI, dots per inch)
- The number of frames (for animated images)
- The creation date and time, and other metadata (if any)

The `identify` command is often used by image processing and manipulation software to display or retrieve image information, especially in batch-processing or automation tasks. It is part of the ImageMagick utility suite, a command-line tool for image editing and conversion. 

## tldr 
 
> Command-line utility of Image Magick project to describe the format and characteristics of one or more image files.
> More information: <https://imagemagick.org/script/identify.php>.

- Describe the format and basic characteristics of an image:

`identify {{path/to/image}}`

- Describe the format and verbose characteristics of an image:

`identify -verbose {{path/to/image}}`

- Collect dimensions of all JPEG files under current directory:

`identify -format "%f,%w,%h\n" *.{{jpg}} > {{path/to/filelist.csv}}`
