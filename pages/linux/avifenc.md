# avifenc 
## chatgpt 
The "avifenc" command is a command-line tool for encoding image sequences or video files to the AV1 Image File Format (AVIF). AVIF is a relatively new image format that provides higher compression efficiency compared to other popular formats like JPEG, PNG or GIF.

When you run the "avifenc" command in a terminal, you need to specify the input file or files that you want to convert to AVIF. This can be a single image file or a video file in a supported format such as MP4, MOV or AVI.

After specifying the input file, you can set several options for the encoding process such as the output file name, the encoding quality, the preferred color profile or whether to use lossless compression or not. You can also set advanced options such as tile size, thread count or speed vs quality tradeoffs.

The resulting AVIF file can be used in modern browsers that support this format, or in specific software that support it, such as image editing or video editing software.

Overall, the "avifenc" command provides a powerful and efficient way to convert image or video files to the newest and most advanced image format available, with the promise of providing better quality and smaller file sizes. 

## tldr 
 
> AV1 Image File Format (AVIF) encoder.
> More information: <https://aomediacodec.github.io/av1-avif/>.

- Convert a specific PNG image to AVIF:

`avifenc {{path/to/image.png}} {{path/to/image.avif}}`

- Encode with a specific speed, where 0=slowest, 10=fastest, and 6=default:

`avifenc --speed {{2}} {{path/to/image.png}} {{path/to/image.avif}}`
