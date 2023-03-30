# astyle 
## chatgpt 
Astyle is a command line tool used for formatting and styling source code files written in C, C++, C#, Java, and Objective-C programming languages. 

When executed, the astyle command will analyze a specified source code file (or multiple files) and reformat them according to the defined formatting rules. These rules can be customized by the user, including settings such as indentation, brace styles, and whitespace.

The astyle command works by modifying the source code directly, rather than creating a new formatted copy. This means that any changes made to the code will be permanent.

Here is an example of how to use the astyle command:

```bash
astyle --style=google myfile.cpp
```

This command will format the "myfile.cpp" file using the Google C++ style guide. Other formatting options include the "kr" style, the "ansi" style, and many more.

Overall, the astyle command is a useful tool for ensuring consistency and readability in code by automatically applying a standardized style. 

## tldr 
 
> Source code indenter, formatter, and beautifier for the C, C++, C# and Java programming languages.
> Upon running, a copy of the original file is created with an ".orig" appended to the original file name.
> More information: <http://astyle.sourceforge.net/>.

- Apply the default style of 4 spaces per indent and no formatting changes:

`astyle {{source_file}}`

- Apply the Java style with attached braces:

`astyle --style=java {{path/to/file}}`

- Apply the allman style with broken braces:

`astyle --style=allman {{path/to/file}}`

- Apply a custom indent using spaces. Choose between 2 and 20 spaces:

`astyle --indent=spaces={{number_of_spaces}} {{path/to/file}}`

- Apply a custom indent using tabs. Choose between 2 and 20 tabs:

`astyle --indent=tab={{number_of_tabs}} {{path/to/file}}`
