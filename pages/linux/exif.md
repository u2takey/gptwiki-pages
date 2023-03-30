# exif 
## chatgpt 
Exif stands for Exchangeable image file format. It is a command that is used to display metadata information of an image file. This metadata includes details such as camera make and model, date and time the photo was taken, shutter speed, aperture, ISO, GPS coordinates, and many other details depending on the camera and the settings used to take the photo.

The exif command works by extracting information stored in the header of the image file, which is known as the Exif data. This data is stored in a standardized format, making it accessible to a wide range of software applications.

The exif command can be used on various operating systems and is often used by photographers and photo editors to get detailed information about photos, such as the camera and lens settings used to capture them.

In addition to displaying metadata, the exif command can also modify some of the metadata, such as adding or changing keywords or captions, rotating the image, or correcting the orientation of the image. However, these options may not be available in all versions of the exif command, and some image file formats may not support modifying the metadata. 

## tldr 
 
> Show and change EXIF information in JPEG files.
> More information: <https://github.com/libexif/exif/>.

- Show all recognized EXIF information in an image:

`exif {{path/to/image.jpg}}`

- Show a table listing known EXIF tags and whether each one exists in an image:

`exif --list-tags --no-fixup {{image.jpg}}`

- Extract the image thumbnail into the file `thumbnail.jpg`:

`exif --extract-thumbnail --output={{thumbnail.jpg}} {{image.jpg}}`

- Show the raw contents of the "Model" tag in the given image:

`exif --ifd={{0}} --tag={{Model}} --machine-readable {{image.jpg}}`

- Change the value of the "Artist" tag to John Smith and save to `new.jpg`:

`exif --output={{new.jpg}} --ifd={{0}} --tag="{{Artist}}" --set-value="{{John Smith}}" --no-fixup {{image.jpg}}`
