# wal 
## chatgpt 
`wal` is a command-line tool used to generate color schemes by analyzing the colors of an image. 

The `wal` command takes an input image file as its argument and then analyzes the colors in the image to create a color scheme that can be used in a variety of applications such as terminal emulators, text editors, and window managers. 

Some of the parameters that can be used with the `wal` command include:

- `-i` or `--iterative`: This option allows you to iteratively apply the color scheme to different applications without having to run the command repeatedly.

- `-s` or `--saturate`: This option increases the saturation of the generated colors.

- `-c` or `--change`: This option changes the wallpaper along with the color scheme.

- `-l` or `--lightness`: This option adjusts the overall lightness of the generated colors.

Once the `wal` command has finished generating the color scheme, it will output the hex values of the colors in the scheme. These values can then be used in your application's configuration file to apply the color scheme. 

## tldr 
 
> A tool to create color schemes based on the dominant colors of a wallpaper.
> More information: <https://github.com/dylanaraps/pywal>.

- Preview color scheme:

`wal --preview {{image.png}}`

- Create color scheme:

`wal -i {{image.png}}`

- Create a light color scheme:

`wal -i {{image.png}} -l`

- Skip setting the desktop wallpaper:

`wal -i {{image.png}} -n`

- Skip setting the terminal colors:

`wal -i {{image.png}} -s`

- Restore the previously generated color scheme and wallpaper:

`wal -R`
