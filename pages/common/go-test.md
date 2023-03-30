# go test 
## chatgpt 
The "go test" command is a testing tool provided by the Go programming language. It is used to execute all the tests that are defined in the Go source code files.

When executed, the "go test" command will search for the test files and test functions in the current directory and its sub-directories. It will automatically compile the test files and execute them to identify any errors or failed tests.

"Go test" command has several options that can be used to customize its behavior. Some of them are:

- "-v" option: To display detailed logs of the test execution.
- "-run" option: To only execute the tests that match a specific regular expression pattern.
- "-bench" option: To run benchmark tests.

Overall, the "go test" command is a powerful tool that allows Go programmers to test their code and ensure that it works as expected in a well-structured and maintained way. 

## tldr 
 
> Tests Go packages (files have to end with `_test.go`).
> More information: <https://golang.org/cmd/go/#hdr-Testing_flags>.

- Test the package found in the current directory:

`go test`

- [v]erbosely test the package in the current directory:

`go test -v`

- Test the packages in the current directory and all subdirectories (note the `...`):

`go test -v ./...`

- Test the package in the current directory and run all benchmarks:

`go test -v -bench .`

- Test the package in the current directory and run all benchmarks for 50 seconds:

`go test -v -bench . -benchtime {{50s}}`

- Test the package with coverage analysis:

`go test -cover`
