# pngcheck 
## chatgpt 
pngcheck is a command-line tool used to validate and verify the integrity of PNG (Portable Network Graphics) image files. It analyzes the PNG file structure, checks for errors, and displays information about the PNG image file. 

The basic syntax of the pngcheck command is:

```
pngcheck [options] <file.png>
```

Here, "file.png" is the name of the PNG image file that you want to check. The command line arguments that are supported by pngcheck are:

1. `-v` or `--verbose`: This option displays comprehensive information about the structure and content of the PNG file.

2. `-f` or `--force`: This option forces pngcheck to ignore certain errors and perform the file analysis. 

3. `-p` or `--print`: This option displays the contents of the PNG file as text.

4. `-c` or `--checksum`: This option calculates and displays the checksums of various parts of the PNG file.

5. `-t` or `--text`: This option displays ancillary text chunks in the PNG file.

6. `-q` or `--quiet`: This option suppresses the normal output of pngcheck and only displays error messages.

Overall, the pngcheck command is a handy tool to identify and correct any issues with the PNG image file and ensure that it meets the required standards. 

## tldr 
 
> Print detailed information about and verify PNG, JNG, and MNG files.
> More information: <http://www.libpng.org/pub/png/apps/pngcheck.html>.

- Print a summary for an image (width, height, and color depth):

`pngcheck {{image.png}}`

- Print information for an image with [c]olorized output:

`pngcheck -c {{image.png}}`

- Print [v]erbose information for an image:

`pngcheck -cvt {{image.png}}`

- Receive an image from `stdin` and display detailed information:

`cat {{path/to/image.png}} | pngcheck -cvt`

- [s]earch for PNGs within a specific file and display information about them:

`pngcheck -s {{image.png}}`

- Search for PNGs within another file and e[x]tract them:

`pngcheck -x {{image.png}}`
