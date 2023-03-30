# magick 
## chatgpt 
magick is a command that is used to invoke the ImageMagick software suite. ImageMagick is a free and open-source software suite used for creating, editing, and converting raster and vector images.

When the magick command is invoked, it launches the ImageMagick software suite and allows you to perform a wide range of image manipulation tasks such as resizing, rotating, cropping, filtering, and more. You can also use the magick command to convert images between different file formats, including BMP, GIF, JPEG, PNG, and TIFF.

To use the magick command, you first need to install the ImageMagick software suite on your system. Once installed, you can use the magick command from the command line or terminal window.

For example, you can use the following command to rotate an image by 90 degrees:

```
magick input-image.jpg -rotate 90 output-image.jpg
```

This command takes an input image "input-image.jpg", rotates it by 90 degrees with the "-rotate 90" option and saves the rotated image as "output-image.jpg".

Overall, the magick command is a powerful tool that allows you to perform a wide range of image manipulation tasks quickly and easily. 

## tldr 
 
> Create, edit, compose, or convert bitmap images.
> ImageMagick version 7+. See `convert` for versions 6 and below.
> More information: <https://imagemagick.org/>.

- Convert file type:

`magick {{image.png}} {{image.jpg}}`

- Resize an image, making a new copy:

`magick convert -resize {{100x100}} {{image.jpg}} {{image.jpg}}`

- Create a GIF using images:

`magick {{*.jpg}} {{images.gif}}`

- Create checkerboard pattern:

`magick -size {{640x480}} pattern:checkerboard {{checkerboard.png}}`

- Convert images to individual PDF pages:

`magick {{*.jpg}} +adjoin {{page-%d.pdf}}`
