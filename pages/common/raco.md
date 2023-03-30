# raco 
## chatgpt 
raco is a command line tool that comes with the Racket programming language. It provides a variety of functionalities for managing Racket packages, running and compiling Racket programs, and interacting with the Racket REPL (read-eval-print loop).

Here are some of the most commonly used sub-commands of raco:

- `raco pkg`: Used for managing Racket packages. Some of the tasks that can be performed using this command include installing and uninstalling packages, creating new packages, upgrading packages, and searching for packages.

- `raco make`: Used for compiling Racket programs. It takes a Racket source file as input and produces a compiled binary that can be executed directly.

- `raco test`: Used for running Racket test suites. This command searches for test files in the specified directory and runs them. It also generates a report with information about the tests that passed and failed.

- `raco doc`: Used for generating documentation for Racket code. This command generates HTML files with information about a package's functions, variables, and syntax.

- `raco repl`: Used for starting a Racket REPL. This is a command line interface that provides an interactive environment for running Racket code.

Overall, raco is a versatile tool that provides developers with many useful functionalities for working with Racket. 

## tldr 
 
> Racket command-line tools.
> More information: <https://docs.racket-lang.org/raco/>.

- Install a package, automatically installing dependencies:

`raco pkg install --auto {{package_source}}`

- Install the current directory as a package:

`raco pkg install`

- Build (or rebuild) bytecode, documentation, executables, and metadata indexes for collections:

`raco setup {{collection1 collection2 ...}}`

- Run tests in files:

`raco test {{path/to/tests1.rkt path/to/tests2.rkt ...}}`

- Search local documentation:

`raco docs {{search_terms ...}}`

- Display help:

`raco help`
