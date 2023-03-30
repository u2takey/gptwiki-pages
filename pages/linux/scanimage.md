# scanimage 
## chatgpt 
The scanimage command is a command-line tool used to scan images with a scanner connected to a computer. When the command is executed, it communicates with the scanner using a scanner driver and initiates the scanning process.

Some of the common options used with scanimage command are:

- --device <devicename> – to specify the name of the scanner device to use for scanning
- --format=(jpeg|png|tiff|pdf) – to specify the format of the scanned image
- --resolution <dpi> – to set the scanning resolution in dots per inch
- --mode=(color|gray|lineart) – to set the color mode of the scanner
- --brightness <value> – to set the brightness setting of the scanner
- --contrast <value> – to set the contrast setting of the scanner
- --source=(ADF|Flatbed) – to set the source from which pages are to be scanned. ADF stands for Automatic Document Feeder and Flatbed is a flat glass surface for scanning.
- --batch=[prefix] – to scan multiple pages in a batch, with the prefix specifying the name of the output files.

When the scanning process is completed, the command saves the scanned image file in the specified file format and location. Scanimage is a simple and powerful tool for scanning documents and images, especially for users who prefer command-line tools. 

## tldr 
 
> Scan images with the Scanner Access Now Easy API.
> More information: <http://sane-project.org/man/scanimage.1.html>.

- List available scanners to ensure the target device is connected and recognized:

`scanimage -L`

- Scan an image and save it to a file:

`scanimage --format={{pnm|tiff|png|jpeg}} > {{path/to/new_image}}`
