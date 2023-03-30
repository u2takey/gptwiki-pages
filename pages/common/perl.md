# perl 
## chatgpt 
"perl" is a command used to run Perl scripts or programs. Perl is a high-level programming language that has been popular in the software development industry for many years, particularly for text processing, system administration, and web development. 

When running the "perl" command, the operating system interprets the given Perl script or program as a set of instructions written in Perl language, and executes them accordingly. By default, Perl programs are run from the command line interface (CLI). 

To execute a Perl script or program using the "perl" command, you need to specify the path to the Perl script or program as an argument in the terminal (or command prompt) window. For example: 

```
$ perl my_perl_script.pl
```

This command will run the "my_perl_script.pl" file located in the current working directory using the Perl interpreter. 

The "perl" command has a number of options and arguments that can be used with it to modify its behavior, such as specifying input and output files, specifying command line arguments to the script, turning warnings and errors on or off, and more. You can find more information on these options by typing "perl --help" in the terminal. 

## tldr 
 
> The Perl 5 language interpreter.
> More information: <https://www.perl.org>.

- Parse and execute a Perl script:

`perl {{script.pl}}`

- Check syntax errors on a Perl script:

`perl -c {{script.pl}}`

- Parse and execute a Perl statement:

`perl -e {{perl_statement}}`

- Run a Perl script in debug mode, using `perldebug`:

`perl -d {{script.pl}}`

- Edit all file lines [i]n-place with a specific replacement [e]xpression, saving a backup with a new extension:

`perl -p -i'.{{extension}}' -e 's/{{regular_expression}}/{{replacement}}/g' {{path/to/file}}`

- Run a multi-line replacement [e]xpression on a file, and save the result in a specific file:

`perl -p -e 's/{{foo\nbar}}/{{foobar}}/g' {{path/to/input_file}} > {{path/to/output_file}}`

- Run a regular [e]xpression on `stdin`, printing matching [l]ines:

`cat {{path/to/file}} | perl -n -l -e 'print if /{{regular_expression}}/'`

- Run a regular [e]xpression on `stdin`, printing only the first capture group for each matching [l]ine:

`cat {{path/to/file}} | perl -n -l -e 'print $1 if /{{before}}({{regular_expression}}){{after}}/'`
