# pixterm 
## chatgpt 
Pixterm is a command used to open a terminal window that displays images directly in the terminal. It allows users to view images in the terminal, without having to open a separate image viewer application.

The command to use pixterm is simply "pixterm" followed by the name and location of the image file that you want to view. For example, if you want to view an image file named "test.jpg" that is located on your desktop, your command would look like this:

pixterm ~/Desktop/test.jpg

Once you enter this command, a new terminal window will open, displaying the image in ASCII art format. You can then use the usual terminal commands to navigate the image, such as scrolling up and down to view different parts of the image.

It's important to note that pixterm requires a terminal emulator that supports the SIXEL graphics protocol, which is used to display the images. So, if you're using a terminal emulator that doesn't support SIXEL, you won't be able to use pixterm. 

## tldr 
 
> Image printing in the terminal.
> See also: `chafa`, `catimg`.
> More information: <https://github.com/eliukblau/pixterm>.

- Render a static image directly in the terminal:

`pixterm {{path/to/file}}`

- Use the image's original aspect ratio:

`pixterm -s 2 {{path/to/file}}`

- Specify a custom aspect ratio using a specific number of [t]erminal [r]ows and [c]olumns:

`pixterm -tr {{24}} -tc {{80}} {{path/to/file}}`

- Filter the output with a [m]atte background color and character [d]ithering:

`pixterm -m {{000000}} -d 2 {{path/to/file}}`
