# svgcleaner 
## chatgpt 
SVG Cleaner is a command-line tool used to clean up SVG files before they are used. It removes unnecessary elements, reduces file size, and converts shapes to simpler forms, making them easier to work with. 

The basic command for SVG Cleaner is: 

```
svgcleaner [input file] [output file]
```

Where [input file] is the path to the original SVG file that needs to be cleaned, and [output file] is the path for the cleaned file to be saved.

Here are some of the additional options that can be used with the command:

`--indent` - writes the output in an indented format.

`--quiet` - disables the standard output and only outputs error messages.

`--precision=[n]` - sets the number of decimal places in the output file.

`--rounding=half|none` - sets the type of rounding to be used.

`--shape-compression` - compresses SVG shapes if possible.

`--verbose` - provides detailed feedback on the cleaning process.

`--preserve-xml-comments` - preserves XML comments in the output file.

Overall, SVG Cleaner is a useful tool for removing unnecessary data and optimizing SVG files for use. 

## tldr 
 
> SVG optimizing utility.
> More information: <https://github.com/RazrFalcon/svgcleaner>.

- Optimize an SVG:

`svgcleaner {{input.svg}} {{output.svg}}`

- Optimize an SVG multiple times:

`svgcleaner --multipass {{input.svg}} {{output.svg}}`
