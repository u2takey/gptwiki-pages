# groff 
## chatgpt 
groff is a command-line tool used for typesetting documents on UNIX and UNIX-like operating systems. It is a powerful program that understands a variety of markup languages like the GNU roff language, LaTeX, and HTML. groff can output to various file formats such as PostScript, PDF, HTML, and plain text.

Typically, to use groff, you would first create a document in one of the supported markup languages. Then, you would run the document through groff, specifying the desired output format and any additional options. groff would then process the document and generate the output file in the desired format.

For example, to convert a document written in the GNU roff language to a PDF file, you could use the following command:

```
groff -ms -Tpdf inputfile.roff > outputfile.pdf
```

Here, `-ms` tells groff to use the classical macro package for typesetting documents, `-Tpdf` specifies the output format as PDF, and `inputfile.roff` is the input file to be processed. The `>` symbol indicates that the output should be redirected to the file `outputfile.pdf`.

Overall, groff is a powerful tool for typesetting professional-looking documents on UNIX-like systems. 

## tldr 
 
> GNU replacement for the `troff` and `nroff` typesetting utilities.
> More information: <https://www.gnu.org/software/groff>.

- Format output for a PostScript printer, saving the output to a file:

`groff {{path/to/input.roff}} > {{path/to/output.ps}}`

- Render a man page using the ASCII output device, and display it using a pager:

`groff -man -T ascii {{path/to/manpage.1}} | less --RAW-CONTROL-CHARS`

- Render a man page into an HTML file:

`groff -man -T html {{path/to/manpage.1}} > {{path/to/manpage.html}}`

- Typeset a roff file containing [t]ables and [p]ictures, using the [me] macro set, to PDF, saving the output:

`groff {{-t}} {{-p}} -{{me}} -T {{pdf}} {{path/to/input.me}} > {{path/to/output.pdf}}`

- Run a `groff` command with preprocessor and macro options guessed by the `grog` utility:

`eval "$(grog -T utf8 {{path/to/input.me}})"`
