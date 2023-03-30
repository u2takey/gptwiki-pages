# clang-tidy 
## chatgpt 
Clang-tidy is a command-line tool that is used to analyse C++ code and to suggest improvements, identify potential bugs or code smells. It uses the Clang compiler infrastructure to parse the source code and the LLVM framework to provide code analysis features. Clang-tidy can be used to detect a wide range of issues such as memory leaks, null pointer dereferences, undefined behaviour, code style violations and many others. The tool can be used directly from the command line, integrated into an IDE or used as a part of a build system. To use the tool, the user specifies the source files they want to analyze as inputs and can choose from a range of pre-defined checks or create their own. Clang-tidy provides a wealth of options for customizing the analysis process, including ignoring certain warnings, specifying additional compiler flags or generating a compilation database. The tool is widely used in the C++ community and is considered an essential part of the modern C++ developer's toolkit. 

## tldr 
 
> An LLVM-based C/C++ linter to find style violations, bugs and security flaws through static analysis.
> More information: <https://clang.llvm.org/extra/clang-tidy/>.

- Run default checks on a source file:

`clang-tidy {{path/to/file.cpp}}`

- Don't run any checks other than the `cppcoreguidelines` checks on a file:

`clang-tidy {{path/to/file.cpp}} -checks={{-*,cppcoreguidelines-*}}`

- List all available checks:

`clang-tidy -checks={{*}} -list-checks`

- Specify defines and includes as compilation options (after `--`):

`clang-tidy {{path/to/file.cpp}} -- -I{{my_project/include}} -D{{definitions}}`
