# inkscape 
## chatgpt 
Inkscape is a command-line tool for creating and editing vector graphics.

When the command "inkscape" is executed in the command-line interface, it launches the Inkscape application.

This allows the user to create or edit vector graphics files, such as SVG (Scalable Vector Graphics) files, using various tools and features provided by Inkscape. These graphics can be used for various purposes, including web design, logo creation, and print design.

Once launched, Inkscape provides a menu bar and toolbars for accessing various features and tools. It also provides a canvas where the graphic can be created or edited.

Inkscape is a powerful tool that provides a variety of drawing and editing tools, including bezier curves, text editing, and layer management. It also supports various file formats, such as PDF, EPS, and PNG.

Overall, the "inkscape" command provides access to an excellent vector graphics tool that can be used for a variety of design purposes. 

## tldr 
 
> An SVG (Scalable Vector Graphics) editing program.
> For Inkscape versions up to 0.92.x, use -e instead of -o.
> More information: <https://inkscape.org>.

- Open an SVG file in the Inkscape GUI:

`inkscape {{filename.svg}}`

- Export an SVG file into a bitmap with the default format (PNG) and the default resolution (96 DPI):

`inkscape {{filename.svg}} -o {{filename.png}}`

- Export an SVG file into a bitmap of 600x400 pixels (aspect ratio distortion may occur):

`inkscape {{filename.svg}} -o {{filename.png}} -w {{600}} -h {{400}}`

- Export the drawing (bounding box of all objects) of an SVG file into a bitmap:

`inkscape {{filename.svg}} -o {{filename.png}} -D`

- Export a single object, given its ID, into a bitmap:

`inkscape {{filename.svg}} -i {{id}} -o {{object.png}}`

- Export an SVG document to PDF, converting all texts to paths:

`inkscape {{filename.svg}} -o {{filename.pdf}} --export-text-to-path`

- Duplicate the object with id="path123", rotate the duplicate 90 degrees, save the file, and quit Inkscape:

`inkscape {{filename.svg}} --select=path123 --verb="{{EditDuplicate;ObjectRotate90;FileSave;FileQuit}}"`
