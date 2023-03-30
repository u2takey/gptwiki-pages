# mogrify 
## chatgpt 
Mogrify is a command line utility that is used to edit, modify and convert multiple image files in one go. The basic syntax of mogrify command is as follows:

mogrify [options] [filename] [filename2...]

Here, [options] are the various parameters that are used to specify the type of editing to be done on the image files. Some of the most commonly used options include resize, crop, grayscale, flip etc.

[filename] and [filename2…] represent the names of the image files that need to be processed. These can be specified either individually or using wildcards.

When the command is executed, mogrify modifies the specified image files and overwrites the original files with the edited images. This means that mogrify command modifies the files in place, without generating any new files.

Mogrify command is basically used to process multiple images in one go, which can save a lot of time and effort. It is particularly useful when you have a large number of images and need to apply the same set of modifications to all of them. 

## tldr 
 
> Perform operations on multiple images, such as resizing, cropping, flipping, and adding effects.
> Changes are applied directly to the original file.
> More information: <https://imagemagick.org/script/mogrify.php>.

- Resize all JPEG images in the directory to 50% of their initial size:

`mogrify -resize {{50%}} {{*.jpg}}`

- Resize all images starting with "DSC" to 800x600:

`mogrify -resize {{800x600}} {{DSC*}}`

- Convert all PNGs in the directory to JPEG:

`mogrify -format {{jpg}} {{*.png}}`

- Halve the saturation of all image files in the current directory:

`mogrify -modulate {{100,50}} {{*}}`

- Double the brightness of all image files in the current directory:

`mogrify -modulate {{200}} {{*}}`
