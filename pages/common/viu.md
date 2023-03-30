# viu 
## chatgpt 
`viu` is a command-line interface (CLI) image viewer tool for the terminal. It is a lightweight, fast, and efficient image viewer that displays your images in full color and high quality directly in your terminal.

The basic syntax of the `viu` command is as follows:

```
viu [OPTIONS] IMAGE_FILE
```

Where `IMAGE_FILE` is the file path of the image you want to view and `OPTIONS` are optional flags that can modify the behavior of the `viu` command.

Some common options include:

- `-h` or `--help`: Displays a help message that describes the available options and how to use them.

- `-s` or `--fit-size`: Sets the maximum size of the displayed image, so that it fits within the specified terminal size. For example, `viu -s 50% image.jpg` will display the image at a maximum size of 50% of your terminal window.

- `-t` or `--transparent`: Enables transparency support for PNG and GIF images. This option can make it easier to view images with transparent backgrounds.

- `-r` or `--random`: Displays a random image from the current directory. This can be a fun and useful way to browse through a collection of images.

Once you have specified the image file and any additional options, the `viu` command will display the image in your terminal. You can use the arrow keys to pan around the image, and use the `q` key to exit the viewer. Additionally, you can use the `+` and `-` keys to zoom in and out of the image, respectively. 

## tldr 
 
> A small command-line application to view images from the terminal.
> More information: <https://github.com/atanunq/viu>.

- Render an image or animated GIF:

`viu {{path/to/file}}`

- Render an image or GIF from the internet using `curl`:

`curl -s {{https://example.com/image.png}} | viu -`

- Render an image with a transparent background:

`viu -t {{path/to/file}}`

- Render an image with a specific width and height in pixels:

`viu -w {{width}} -h {{height}} {{path/to/file}}`

- Render an image or GIF and display its file name:

`viu -n {{path/to/file}}`
