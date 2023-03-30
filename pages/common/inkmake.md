# inkmake 
## chatgpt 
As an AI language model, I'm not sure what specific tool or application you are referring to with "inkmake." However, based on the term "make," it could be a command used to build or compile files, typically in a software development or programming context. 

The "make" command automates the process of building executable files or libraries from source code, by reading a set of instructions (often written in a Makefile) and performing the necessary tasks to build the desired output. This can involve compiling source code into object files, linking object files to create an executable or library, and various other tasks like copying files, generating documentation, or running tests.

The "ink" part of "inkmake" suggests it may be related to software or systems for printing. However, without more context or information, it's difficult to provide a more detailed explanation. 

## tldr 
 
> GNU Makefile-style SVG exporting using Inkscape's backend.
> More information: <https://github.com/wader/inkmake>.

- Export an SVG file executing the specified Inkfile:

`inkmake {{path/to/Inkfile}}`

- Execute an Inkfile and show detailed information:

`inkmake --verbose {{path/to/Inkfile}}`

- Execute an Inkfile, specifying SVG input file(s) and an output file:

`inkmake --svg {{path/to/file.svg}} --out {{path/to/output_image}} {{path/to/Inkfile}}`

- Specify a custom Inkscape binary to use as the backend:

`inkmake --inkscape {{/Applications/Inkscape.app/Contents/Resources/bin/inkscape}} {{path/to/Inkfile}}`

- Display help:

`inkmake --help`
