# convert 
## chatgpt 
The "convert" command is a versatile image manipulation tool available in Unix and Linux-based systems. This command can perform various conversions and transformations on images, such as resizing, cropping, rotating, adjusting color hues, and many more.

Here are some examples of using the "convert" command:

1. Resizing an image:
The command "convert input.jpg -resize 50% output.jpg" will shrink an image represented by "input.jpg" by 50% and save the resulting image as "output.jpg".

2. Converting an image to a different format:
The command "convert input.png output.jpg" will convert an image represented by "input.png" to a JPEG format and save it as "output.jpg".

3. Adding a watermark to an image:
The command "convert input.jpg -font Arial -pointsize 30 -draw 'gravity south fill black text 0,12 "SAMPLE WATERMARK" fill white text 1,11 "SAMPLE WATERMARK"' output.jpg" adds a watermark to an image represented by "input.jpg". The resulting image is saved as "output.jpg".

Overall, the "convert" command is a powerful tool for image manipulation and conversion, and it can perform various tasks that can help in processing and enhancing images for different applications. 

## tldr 
 
> ImageMagick image conversion tool.
> More information: <https://imagemagick.org/script/convert.php>.

- Convert an image from JPG to PNG:

`convert {{image.jpg}} {{image.png}}`

- Scale an image 50% its original size:

`convert {{image.png}} -resize 50% {{image2.png}}`

- Scale an image keeping the original aspect ratio to a maximum dimension of 640x480:

`convert {{image.png}} -resize 640x480 {{image2.png}}`

- Horizontally append images:

`convert {{image1.png}} {{image2.png}} {{image3.png}} +append {{image123.png}}`

- Vertically append images:

`convert {{image1.png}} {{image2.png}} {{image3.png}} -append {{image123.png}}`

- Create a GIF from a series of images with 100ms delay between them:

`convert {{image1.png}} {{image2.png}} {{image3.png}} -delay {{10}} {{animation.gif}}`

- Create an image with nothing but a solid background:

`convert -size {{800x600}} "xc:{{#ff0000}}" {{image.png}}`

- Create a favicon from several images of different sizes:

`convert {{image1.png}} {{image2.png}} {{image3.png}} {{image.ico}}`
