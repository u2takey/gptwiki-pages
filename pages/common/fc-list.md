# fc-list 
## chatgpt 
The "fc-list" command is used to list all available fonts that are currently installed on the system. This command can help users to check the fonts that are available on their system and choose the appropriate font for their needs. 

When the "fc-list" command is executed, it searches the system for fonts using the FontConfig library. This library is responsible for managing fonts on Linux and other Unix-based systems. It collects information about fonts from various sources, including system files and directories, and stores this information in a configuration file. 

The "fc-list" command reads the configuration file provided by the FontConfig library and displays the result in the console. The output of this command lists all available fonts, including their names, styles, and file locations. This output can be useful for developers and designers who need to work with fonts in their projects. 

For example, the output might look like this:

DejaVu Sans,DejaVu Sans Bold:style=Bold
/usr/share/fonts/truetype/dejavu/DejaVuSans-Bold.ttf: DejaVu Sans,DejaVu Sans Bold:style=Bold
DejaVu Sans:style=Bold Italic
/usr/share/fonts/truetype/dejavu/DejaVuSans-BoldOblique.ttf: DejaVu Sans,DejaVu Sans Bold:style=Italic
DejaVu Sans:style=Oblique
/usr/share/fonts/truetype/dejavu/DejaVuSans-Oblique.ttf: DejaVu Sans,DejaVu Sans:style=Bold Italic
DejaVu Serif:style=Bold
/usr/share/fonts/truetype/dejavu/DejaVuSerif-Bold.ttf: DejaVu Serif,DejaVu Serif Serif Bold:style=Bold

In this example, the font DejaVu Sans is listed multiple times with different styles and file locations. The styles are specified using keywords such as "Bold" or "Italic". The font file locations are also provided, making it easy to identify the files containing the fonts. 

Overall, the "fc-list" command is a useful tool for managing fonts on Linux and other Unix-based systems. It provides a quick and easy way to check available fonts and their details. 

## tldr 
 
> List available fonts installed on the system.
> More information: <https://manned.org/fc-list>.

- Return a list of installed fonts in your system:

`fc-list`

- Return a list of installed fonts with given name:

`fc-list | grep '{{DejaVu Serif}}'`

- Return the number of installed fonts in your system:

`fc-list | wc -l`
