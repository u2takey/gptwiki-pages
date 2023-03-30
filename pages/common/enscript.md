# enscript 
## chatgpt 
The enscript command is a command-line tool that converts plain text files into PostScript language files. It is primarily used for printing and formatting text files for further processing. 

The general syntax of the enscript command is as follows:

```
enscript [options] [files]
```

Where the "options" are the various parameters and settings used to customize the output format, and the "files" are the names of the text files that you want to convert.

Some of the most commonly used options include:

- `-f fontname` - sets the font to be used for the output text
- `-h` - prints a header at the top of each page
- `-o filename.ps` - specifies the name of the output file
- `-p filename.prn` - directs the output to a printer instead of a file
- `-r` - prints in landscape orientation
- `-2r` - prints in two-column format

Overall, the enscript command is a powerful tool for manipulating text files, and its many options make it highly customizable to suit your needs. 

## tldr 
 
> Convert text files to PostScript, HTML, RTF, ANSI, and overstrikes.
> More information: <https://www.gnu.org/software/enscript>.

- Generate a PostScript file from a text file:

`enscript {{path/to/input_file}} --output={{path/to/output_file}}`

- Generate a file in a different language than PostScript:

`enscript {{path/to/input_file}} --language={{html|rtf|...}} --output={{path/to/output_file}}`

- Generate a PostScript file with a landscape layout, splitting the page into columns (maximum 9):

`enscript {{path/to/input_file}} --columns={{num}} --landscape --output={{path/to/output_file}}`

- Display available syntax highlighting languages and file formats:

`enscript --help-highlight`

- Generate a PostScript file with syntax highlighting and color for a specified language:

`enscript {{path/to/input_file}} --color=1 --highlight={{language}} --output={{path/to/output_file}}`
