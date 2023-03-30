# feh 
## chatgpt 
feh is a command-line program used for displaying and managing images on Linux-based operating systems. It provides a simple and lightweight solution for viewing images and can be used to browse through images, set desktop wallpapers, and even create image slideshows.

Some of the common uses of the feh command are:

1. Display an image: You can use the command "feh <image_path>" to display any image in your terminal.

2. View a directory of images: You can use "feh <directory_path>" to open a directory of images in a slideshow format. You can move through images using the arrow keys.

3. Set a desktop wallpaper: You can use "feh --bg-max <image_path>" to set an image as your desktop wallpaper.

By default, feh uses an X11 display server to display images. However, you can also use it in a variety of custom configurations, including displaying images on remote servers over SSH connections, displaying images in full-screen mode, or using different image file formats.

Overall, feh is a powerful and versatile tool that can help you manage and view images on Linux systems quickly and efficiently. 

## tldr 
 
> Lightweight image viewing utility.
> More information: <https://feh.finalrewind.org>.

- View images locally or using a URL:

`feh {{path/to/images}}`

- View images recursively:

`feh --recursive {{path/to/images}}`

- View images without window borders:

`feh --borderless {{path/to/images}}`

- Exit after the last image:

`feh --cycle-once {{path/to/images}}`

- Set the slideshow cycle delay:

`feh --slideshow-delay {{seconds}} {{path/to/images}}`

- Set your wallpaper (centered, filled, maximized, scaled or tiled):

`feh --bg-{{center|fill|max|scale|tile}} {{path/to/image}}`

- Create a montage of all images within a directory. Outputs as a new image:

`feh --montage --thumb-height {{150}} --thumb-width {{150}} --index-info "{{%nn%wx%h}}" --output {{path/to/montage_image.png}}`
