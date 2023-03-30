# exiftool 
## chatgpt 
Exiftool is a command line tool that is used to read, write, and edit the metadata information embedded in various types of files such as images, audio, and video files. The metadata information includes the details about the creation date, camera model, GPS location, and many other properties of the file. 

The syntax for using exiftool is as follows:

exiftool [OPTIONS] [FILE]

Here, [OPTIONS] are the various command line options that can be used to perform different actions on the metadata information of the file, and [FILE] is the path or name of the file on which the command is to be executed.

Some of the commonly used options are:

- -h: This option is used to display the output in a human-readable format.
- -a: This option is used to print all available metadata information.
- -d: This option is used to specify the date format in the output.
- -r: This option is used to recursively process all the files in a directory and its subdirectories.
- -w: This option is used to write the modified metadata information back to the file.

For example, to display all the metadata information of a JPEG image named "example.jpg", the command would be:

exiftool -a example.jpg

This would display all the available metadata information of the image in a human-readable format. 

## tldr 
 
> Read and write meta information in files.
> More information: <https://exiftool.org>.

- Print the EXIF metadata for a given file:

`exiftool {{path/to/file}}`

- Remove all EXIF metadata from the given files:

`exiftool -All= {{path/to/file1 path/to/file2 ...}}`

- Remove GPS EXIF metadata from given image files:

`exiftool "-gps*=" {{path/to/image1 path/to/image2 ...}}`

- Remove all EXIF metadata from the given image files, then re-add metadata for color and orientation:

`exiftool -All= -tagsfromfile @ -colorspacetags -orientation {{image1 image2 ...}}`

- Move the date at which all photos in a directory were taken 1 hour forward:

`exiftool "-AllDates+=0:0:0 1:0:0" {{path/to/directory}}`

- Move the date at which all JPEG photos in the current directory were taken 1 day and 2 hours backward:

`exiftool "-AllDates-=0:0:1 2:0:0" -ext jpg`

- Only change the `DateTimeOriginal` field subtracting 1.5 hours, without keeping backups:

`exiftool -DateTimeOriginal-=1.5 -overwrite_original`

- Recursively rename all JPEG photos in a directory based on the `DateTimeOriginal` field:

`exiftool '-filename<DateTimeOriginal' -d %Y-%m-%d_%H-%M-%S%%lc.%%e {{path/to/directory}} -r -ext jpg`
