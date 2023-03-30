# lilypond 
## chatgpt 
Lilypond is a command-line program used for creating high-quality sheet music from plain text input files written in the Lilypond programming language. The Lilypond program converts the text input file into a printable sheet music document in PDF format.

Some important features and uses of the Lilypond command are:

1. Creation of sheet music: The main use of the Lilypond command is to create high-quality sheet music from plain text input files. This allows users to create professional-looking music notation with complete control over every aspect of the music score, including the layout, fonts, and engraved appearance.

2. Integration with text editors: Lilypond can be used with text editors like Emacs or Vim, allowing users to write Lilypond code directly in the editor and then compile it into sheet music.

3. Automation and batch processing: Lilypond commands can be combined with other programs or scripts to automate the process of creating multiple sheet music files or processing large amounts of data.

4. Support for music notation: Lilypond supports a wide range of music notation, including standard western notation, early music notation, and non-standard notation. It also includes support for lyrics, chord symbols, and rhythmic notation.

5. Customization: Lilypond allows users to customize every aspect of the sheet music output, including the spacing, font size, and layout. This provides users with complete control over the printed output and the ability to create unique and distinctive music scores. 

## tldr 
 
> Typeset music and/or produce MIDI from file.
> More information: <https://lilypond.org>.

- Compile a lilypond file into a PDF:

`lilypond {{path/to/file}}`

- Compile into the specified format:

`lilypond --formats={{format_dump}} {{path/to/file}}`

- Compile the specified file, suppressing progress updates:

`lilypond -s {{path/to/file}}`

- Compile the specified file, and also specify the output filename:

`lilypond --output={{path/to/output_file}} {{path/to/input_file}}`

- Show the current version of lilypond:

`lilypond --version`
