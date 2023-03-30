# bison 
## chatgpt 
Bison is a command-line tool and parser generator used to generate parsing code for computer programs. It is often used with the GNU Compiler Collection (GCC) to parse source code written in the C and C++ programming languages.

When a developer uses Bison, they typically start by writing a formal grammar specification for the target language or file format they want to parse. The Bison tool then takes this grammar and generates a parser in C or C++, which can be compiled into an executable or library.

The generated parser can then be used to parse source code or other input files conforming to the specified grammar, helping the compiler or other program understand and manipulate the data.

In short, the Bison command is used to generate parsing code for C and C++ programs, based on a specified grammar specification. 

## tldr 
 
> GNU parser generator.
> More information: <https://www.gnu.org/software/bison/>.

- Compile a bison definition file:

`bison {{path/to/file.y}}`

- Compile in debug mode, which causes the resulting parser to write additional information to the standard output:

`bison --debug {{path/to/file.y}}`

- Specify the output filename:

`bison --output {{path/to/output.c}} {{path/to/file.y}}`

- Be verbose when compiling:

`bison --verbose`
