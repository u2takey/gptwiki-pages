# gifsicle 
## chatgpt 
Gifsicle is a command line tool used for creating, editing and optimizing animated GIF images. It is a free and open-source software available for Linux, macOS and Windows operating systems. The command 'gifsicle' is basically the name of the executable file that is used to run the tool in the terminal or command prompt.

The gifsicle command can be used for a variety of purposes such as optimizing animated GIFs, cropping, resizing, and manipulating the frames of animated images, adding text overlays, and more. The command is followed by a set of options and arguments that determine the specific task that the user wishes to achieve.

Some common options used with gifsicle include:

- -O: This option is used for optimizing GIFs by reducing their file size without compromising on their image quality.

- --delay: This option allows the user to set the delay time between animation frames in milliseconds.

- --crop: This option is used to crop a portion of the GIF image.

- --resize: This option is used to resize the GIF image to a specific width and height.

- --unoptimize: This option is used to remove the optimization from the GIF image.

Overall, gifsicle is a powerful and versatile tool for working with animated GIF images and can be used for various purposes depending on the user's requirements. 

## tldr 
 
> GIF manipulator.
> More information: <https://www.lcdf.org/gifsicle>.

- Optimize a GIF as a new file:

`gifsicle {{path/to/input.gif}} --optimize=3 -o {{path/to/output.gif}}`

- Unoptimize a GIF in place:

`gifsicle -b {{path/to/input.gif}} --unoptimize`

- Extract a frame from a GIF:

`gifsicle {{path/to/input.gif}} '#{{0}}' > {{path/to/firstframe.gif}}`

- Make a GIF animation from selected GIFs:

`gifsicle {{*.gif}} --delay={{10}} --loop > {{path/to/output.gif}}`

- Reduce file size using lossy compression:

`gifsicle -b {{path/to/input.gif}} --optimize=3 --lossy={{100}} --colors={{16}} --dither`

- Delete the first 10 frames and all frames after frame 20 from a GIF:

`gifsicle -b {{path/to/input.gif}} --delete '#{{0-9}}' '#{{20-}}'`

- Modify all frames of a GIF using specific transformation options:

`gifsicle -b --crop {{50}},{{50}}+{{-50}}x{{-50}} --scale {{0.25}} --flip-horizontal --rotate-90 {{path/to/input.gif}}`
