# uncrustify 
## chatgpt 
Uncrustify is a command-line tool that reformats code written in various programming languages, including C, C++, Objective-C, and others. The tool takes in your source code as input, applies a set of predefined formatting rules, and outputs the reformatted code. This can help improve code readability, consistency, and maintainability.

The uncrustify command is used to run the Uncrustify tool. When running the command, you will typically need to provide the file or directory containing the code you want to format, as well as any options or configuration settings you want to use. Some common options include setting the output format (e.g., tabs or spaces), specifying the maximum line length, and controlling how certain code constructs are formatted (e.g., curly braces placement).

Here is an example usage of the uncrustify command:

```
uncrustify -c my_config.cfg -f my_code.cpp -o my_formatted_code.cpp
```

In this example, we are telling Uncrustify to use the configuration file "my_config.cfg" to format the input file "my_code.cpp". The reformatted code will be output to a new file called "my_formatted_code.cpp". Note that there are many other options and configuration settings that can be provided to the uncrustify command depending on your specific needs. 

## tldr 
 
> C, C++, C#, D, Java and Pawn source code formatter.
> More information: <https://github.com/uncrustify/uncrustify>.

- Format a single file:

`uncrustify -f {{path/to/file.cpp}} -o {{path/to/output.cpp}}`

- Read filenames from `stdin`, and take backups before writing output back to the original filepaths:

`find . -name "*.cpp" | uncrustify -F - --replace`

- Don't make backups (useful if files are under version control):

`find . -name "*.cpp" | uncrustify -F - --no-backup`

- Use a custom configuration file and write the result to `stdout`:

`uncrustify -c {{path/to/uncrustify.cfg}} -f {{path/to/file.cpp}}`

- Explicitly set a configuration variable's value:

`uncrustify --set {{option}}={{value}}`

- Generate a new configuration file:

`uncrustify --update-config -o {{path/to/new.cfg}}`
