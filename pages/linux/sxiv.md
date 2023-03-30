# sxiv 
## chatgpt 
sxiv is a command-line based image viewer that allows users to easily browse and view images. The following are some basic details about the command:

1. Installation: The command can be installed on Unix-like operating systems such as Linux and macOS using the package manager of the respective distribution.

2. Usage: The command can be invoked by typing 'sxiv' followed by the name of the desired image file or a directory containing multiple image files. The user interface of the viewer includes features such as zooming, panning, and thumbnail previews.

3. Customization: The viewer allows users to customize various aspects of the interface such as key-bindings, image resizing options, and color schemes. These customizations can be made by modifying the configuration file of the program.

4. Advanced features: The viewer also includes features such as slideshow mode, image rotation, and full-screen viewing. Additionally, it allows users to sort and filter images based on various criteria such as file size and creation date.

Overall, sxiv is a versatile and useful command-line tool for browsing and viewing images on Unix-like systems. 

## tldr 
 
> Simple X Image Viewer.
> More information: <https://github.com/muennich/sxiv>.

- Open an image:

`sxiv {{path/to/file}}`

- Open an image in fullscreen mode:

`sxiv -f {{path/to/file}}`

- Open a newline-separated list of images, reading filenames from standard input:

`echo {{path/to/file}} | sxiv -i`

- Open a space-separated list of images as a slideshow:

`sxiv -S {{seconds}} {{path/to/file}}`

- Open a space-separated list of images in thumbnail mode:

`sxiv -t {{path/to/file}}`
