# cppcheck 
## chatgpt 
cppcheck is a command-line tool used for static analysis of C/C++ code. It detects and flags errors, warnings, and potential bugs in the source code of these programming languages. 

To use the cppcheck command, you need to install it first on your system. Here are the steps to install cppcheck on Linux systems:

1. Open the terminal and run the following command to update the package list:

        sudo apt-get update

2. Run the following command to install cppcheck:

        sudo apt-get install cppcheck

Once you have cppcheck installed, you can use the following command to analyze a C/C++ code file:

    cppcheck <file_name>

Replace <file_name> with the name of your C/C++ code file. The cppcheck command analyzes the file and returns a list of warnings and errors that need to be fixed in the code.

You can also use the following additional options with the cppcheck command:

- `-j <number_of_threads>`: This option lets you perform parallel analysis of multiple files. Specify the number of threads to use for analysis.

- `--enable=<check_name>`: This option lets you enable a particular check such as nullpointer, style, or unusedFunction. 

- `--xml`: This option generates the output in XML format.

Overall, the cppcheck command is a useful tool for catching errors and potential bugs in your C/C++ code before you compile and run it. 

## tldr 
 
> A static analysis tool for C/C++ code.
> Instead of syntax errors, it focuses on the types of bugs that compilers normally do not detect.
> More information: <http://cppcheck.sourceforge.net>.

- Recursively check the current directory, showing progress on the screen and logging error messages to a file:

`cppcheck . 2> cppcheck.log`

- Recursively check a given directory, and don't print progress messages:

`cppcheck --quiet {{path/to/directory}}`

- Check a given file, specifying which tests to perform (by default only errors are shown):

`cppcheck --enable={{error|warning|style|performance|portability|information|all}} {{path/to/file.cpp}}`

- List available tests:

`cppcheck --errorlist`

- Check a given file, ignoring specific tests:

`cppcheck --suppress={{test_id1}} --suppress={{test_id2}} {{path/to/file.cpp}}`

- Check the current directory, providing paths for include files located outside it (e.g. external libraries):

`cppcheck -I {{include/directory_1}} -I {{include/directory_2}} .`

- Check a Microsoft Visual Studio project (`*.vcxproj`) or solution (`*.sln`):

`cppcheck --project={{path/to/project.sln}}`
