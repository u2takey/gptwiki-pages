# ctest 
## chatgpt 
The `ctest` command is a part of the CMake build system and is used to run tests on the project. It is used to invoke CMake generated test executables and report the results. 

When a CMake project is built, `CTest` automatically generates a list of tests based on the tests defined in the CMakeLists.txt file. The `ctest` command then executes the tests and reports the results in a consolidated format that can be easily reviewed.

Here are some of the common options and arguments that can be passed to the `ctest` command:

- `-R <regex>`: Run tests that match the given regular expression.
- `-L <label>`: Run tests that have the specified label.
- `-E <regex>`: Exclude tests that match the given regular expression.
- `-VV`: Increase the verbosity level of the test output.
- `-j <jobs>`: Number of tests to run in parallel.

Overall, `ctest` helps to simplify the process of testing and verifying the functionality of CMake projects. 

## tldr 
 
> CMake test driver program.
> More information: <https://gitlab.kitware.com/cmake/community/wikis/doc/ctest/Testing-With-CTest>.

- Run all tests defined in the CMake project, executing 4 jobs at a time in parallel:

`ctest -j{{4}} --output-on-failure`

- Show a list of available tests:

`ctest -N`

- Run a single test based on its name, or filter on a regular expression:

`ctest --output-on-failure -R '^{{test_name}}$'`
