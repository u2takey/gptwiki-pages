# montage 
## chatgpt 
Montage is a command-line tool used to create a multi-image composite by combining multiple separate image files into a single composite image. The montage command comes with the ImageMagick suite of command-line image processing tools.

To use the montage command, you need to have ImageMagick installed on your system. Once installed, you can open a terminal or command prompt and enter the following syntax:

montage [options] input-files output-file

- [options] refer to any additional options or settings you want to apply when creating the composite image.
- input-files refer to the list of image files you want to combine.
- output-file is the filename of the composite image you want to create.

Some of the most common options available with the montage command include:

- -mode: Specifies the type of color reduction or merging used to create the composite image, for example, grayscale or RGB.
- -geometry: Sets the width and height of the individual images in the composite.
- -tile: Determines the number of rows and columns to use for arranging the images, for instance, 2x3 means two rows and three columns.
- -frame: Adds a border or frame around each image in the composite.

Overall, using the montage command allows you to create a visually appealing, well-organized composite image containing multiple images in just a single step. 

## tldr 
 
> ImageMagick image montage tool.
> Tiles images into a customisable grid.
> More information: <https://imagemagick.org/script/montage.php>.

- Tile images into a grid, automatically resizing images larger than the grid cell size:

`montage {{image1.png}} {{image2.jpg}} {{imageN.png}} montage.jpg`

- Tile images into a grid, automatically calculating the grid cell size from the largest image:

`montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry +0+0 montage.jpg`

- Set the grid cell size and resize images to fit it before tiling:

`montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry 640x480+0+0 montage.jpg`

- Limit the number of rows and columns in the grid, causing input images to overflow into multiple output montages:

`montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry +0+0 -tile 2x3 montage_%d.jpg`

- Resize and crop images to fill their grid cells before tiling:

`montage {{image1.png}} {{image2.jpg}} {{imageN.png}} -geometry +0+0 -resize 640x480^ -gravity center -crop 640x480+0+0 montage.jpg`
