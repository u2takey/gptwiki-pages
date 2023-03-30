# guetzli 
## chatgpt 
Guetzli is a command-line tool used for image compression. It was developed by Google and released in 2017. The tool uses a psychovisual model to compress JPEG and PNG images without losing image quality. 

When using the Guetzli command, you provide the input image file and desired output file as arguments. For example, the command might look like:

```
guetzli input.jpg output.jpg
```

The tool will then use a combination of color quantization and the psychovisual model to compress the image. The output file will be smaller in size while maintaining the same level of image quality.

There are several optional parameters that can be used with the Guetzli command. These include:

- quality: This parameter specifies the JPEG quality of the output image. The default value is 95 but can be set to any value between 84 and 100.

- butteraugli_target: This parameter specifies the maximum difference in image quality that can be tolerated. The default value is 1.0 and can be adjusted depending on your tolerance for image quality loss.

Overall, Guetzli is useful for reducing the file size of images without sacrificing image quality. 

## tldr 
 
> JPEG image compression utility.
> More information: <https://github.com/google/guetzli>.

- Compress a JPEG image:

`guetzli {{input.jpg}} {{output.jpg}}`

- Create a compressed JPEG from a PNG:

`guetzli {{input.png}} {{output.jpg}}`

- Compress a JPEG with the desired visual quality (84-100):

`guetzli --quality {{quality_value}} {{input.jpg}} {{output.jpg}}`
