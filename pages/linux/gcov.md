# gcov 
## chatgpt 
`gcov` is a command-line utility that is used to measure and report the code coverage of C and C++ programs.

When you run a program with the `gcov` command, it generates a set of files that provide information about how much of the program's executable code has been executed during the tests. These files are called coverage data files and typically have the extension `.gcda`.

You can use the `gcov` command to analyze these data files and generate a report that shows how much of the code has been executed and which lines have not been executed. The report includes information such as the number of times each line of code was executed, the percentage of lines executed, and the number of times each function was called.

In general, code coverage analysis is an important tool for software developers to identify and fix defects in their code. By using `gcov` to measure and analyze code coverage, developers can identify areas of their code that are not being tested sufficiently and take steps to improve the overall quality of their software. 

## tldr 
 
> Code coverage analysis and profiling tool that discovers untested parts of a program.
> Also displays a copy of source code annotated with execution frequencies of code segments.
> More information: <https://gcc.gnu.org/onlinedocs/gcc/Invoking-Gcov.html>.

- Generate a coverage report named `file.cpp.gcov`:

`gcov {{path/to/file.cpp}}`

- Write individual execution counts for every basic block:

`gcov --all-blocks {{path/to/file.cpp}}`

- Write branch frequencies to the output file and print summary information to `stdout` as a percentage:

`gcov --branch-probabilities {{path/to/file.cpp}}`

- Write branch frequencies as the number of branches taken, rather than the percentage:

`gcov --branch-counts {{path/to/file.cpp}}`

- Do not create a `gcov` output file:

`gcov --no-output {{path/to/file.cpp}}`

- Write file level as well as function level summaries:

`gcov --function-summaries {{path/to/file.cpp}}`
