# pytest 
## chatgpt 
The command "pytest" is used to execute tests written in Python using the pytest testing framework. It searches for test files in the current directory and its subdirectories, and runs the test functions contained in them.

When running the "pytest" command, the following things can happen:

1. pytest automatically discovers and executes any files in the current directory or its subdirectories that are named with the pattern "test_*.py" or "*_test.py".
2. By default, pytest runs all tests it finds, but you can specify one or more test files to run by listing them after the "pytest" command. For example, "pytest test_file.py" would only run tests found in the "test_file.py" file.
3. pytest displays the results of the tests in a colored output format that makes it easy to see which tests passed and which ones failed.
4. Pytest also provides several useful command line options that can be used to control the execution of tests, such as "--verbose" to display more detailed output or "-k" to run only tests that match a specific keyword.

Overall, the "pytest" command is an essential tool for Python developers who want to write and run automated tests to ensure the quality and reliability of their code. 

## tldr 
 
> Run Python tests.
> More information: <https://docs.pytest.org/>.

- Run tests from specific files:

`pytest {{path/to/test_file1.py path/to/test_file2.py ...}}`

- Run tests with names matching a specific [k]eyword expression:

`pytest -k {{expression}}`

- Exit as soon as a test fails or encounters an error:

`pytest --exitfirst`

- Run tests matching or excluding markers:

`pytest -m {{marker_name1 and not marker_name2}}`

- Run until a test failure, continuing from the last failing test:

`pytest --stepwise`

- Run tests without capturing output:

`pytest --capture=no`
