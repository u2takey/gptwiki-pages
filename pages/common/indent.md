# indent 
## chatgpt 
The `indent` command is a Linux command used to modify the indentation of the given file(s). It formats the source code and ensures that it follows a certain convention in terms of indentation, with the aim of improving its readability and structure. The command is generally used for code written in languages like C, C++, Java, Python, and others.

The `indent` command can be used with various options to specify the formatting style and other parameters. Some of the common options are:

- `-kr` option to use the Kernighan and Ritchie (K&R) style of indentation.
- `-linux` option to use the Linux kernel style of indentation.
- `-gnu` option to use the GNU style of indentation.
- `-ts` option to specify the tab size to use for indentation.

The command can be used on a single file or a group of files using regular expressions or wildcards. For example, to indent all C source files in the current directory and its subdirectories, you can use:

```
$ indent -kr *.c
```

This will use the K&R style of indentation and format all the C source files (*.c) in the current directory and its subdirectories.

Overall, the `indent` command is a useful tool for formatting and improving the structure and readability of source code. 

## tldr 
 
> Change the appearance of a C/C++ program by inserting or deleting whitespace.
> More information: <https://www.gnu.org/software/indent/>.

- Format C/C++ source according to the Linux style guide, automatically back up the original files, and replace with the indented versions:

`indent --linux-style {{path/to/source.c}} {{path/to/another_source.c}}`

- Format C/C++ source according to the GNU style, saving the indented version to a different file:

`indent --gnu-style {{path/to/source.c}} -o {{path/to/indented_source.c}}`

- Format C/C++ source according to the style of Kernighan & Ritchie (K&R), no tabs, 3 spaces per indent, and wrap lines at 120 characters:

`indent --k-and-r-style --indent-level3 --no-tabs --line-length120 {{path/to/source.c}} -o {{path/to/indented_source.c}}`
