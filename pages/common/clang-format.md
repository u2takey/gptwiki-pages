# clang-format 
## chatgpt 
Clang-format is a command line tool that is used to automatically format source code written in C++, C, Obj-C, or ProtoBuf. It is a part of the Clang project and uses Clang's parsing engine to create a formatted output of the code. 

Clang-format can be run with a variety of options to customize the formatting, such as specifying the indentation level, line wrapping rules, and how to handle comments in the code. 

Some common use cases include using clang-format to automatically format code before committing changes to a version control system, or integrating it into a continuous integration pipeline to ensure consistent code formatting across a team. 

Overall, clang-format is a powerful command line tool that can save developers time and effort when it comes to formatting code, and can help maintain consistency and readability in large code repositories. 

## tldr 
 
> Tool to auto-format C/C++/Java/JavaScript/Objective-C/Protobuf/C# code.
> More information: <https://clang.llvm.org/docs/ClangFormat.html>.

- Format a file and print the result to `stdout`:

`clang-format {{path/to/file}}`

- Format a file in-place:

`clang-format -i {{path/to/file}}`

- Format a file using a predefined coding style:

`clang-format --style={{LLVM|GNU|Google|Chromium|Microsoft|Mozilla|WebKit}} {{path/to/file}}`

- Format a file using the `.clang-format` file in one of the parent directories of the source file:

`clang-format --style=file {{path/to/file}}`

- Generate a custom `.clang-format` file:

`clang-format --style={{LLVM|GNU|Google|Chromium|Microsoft|Mozilla|WebKit}} --dump-config > {{.clang-format}}`
