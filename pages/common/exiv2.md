# exiv2 
## chatgpt 
exiv2 is a command-line utility for managing image metadata. It allows users to view, edit, and modify various types of image metadata, including EXIF, IPTC, and XMP data.

The basic syntax for using exiv2 is:

`exiv2 [options] [command] [file(s)]`

Here, options are any optional flags or settings that can be passed to the command, e.g. -v for verbose output. Command is the action to be performed, such as "print" for displaying the metadata of an image. File(s) are the image file(s) or directory to be processed, with wildcard characters supported.

Some common exiv2 commands include:

- `print`: Displays the metadata of one or more images, including EXIF, IPTC, and XMP data.
- `extract`: Copies metadata from one image to another, or from an image to a text file.
- `write`: Modifies the metadata of one or more images.
- `rename`: Renames image files according to their metadata, such as the date and time the photo was taken.
- `restore`: Recovers metadata from backup files after an image has been modified.

Overall, exiv2 provides a powerful set of tools for managing image metadata from the command line. It can be especially useful for batch processing large numbers of images, or for incorporating metadata management into automated workflows. 

## tldr 
 
> Image metadata manipulation tool.
> More information: <https://www.exiv2.org/manpage.html>.

- Print a summary of the image Exif metadata:

`exiv2 {{path/to/file}}`

- Print all metadata (Exif, IPTC, XMP) with interpreted values:

`exiv2 -P kt {{path/to/file}}`

- Print all metadata with raw values:

`exiv2 -P kv {{path/to/file}}`

- Delete all metadata from an image:

`exiv2 -d a {{path/to/file}}`

- Delete all metadata, preserving the file timestamp:

`exiv2 -d a -k {{path/to/file}}`

- Rename the file, prepending the date and time from metadata (not from the file timestamp):

`exiv2 -r {{'%Y%m%d_%H%M%S_:basename:'}} {{path/to/file}}`
