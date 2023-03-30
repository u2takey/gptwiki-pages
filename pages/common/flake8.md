# flake8 
## chatgpt 
The "flake8" command is a tool used for checking Python code for potential errors and style issues. It is a combination of several other tools: "PyFlakes," "pep8," and "mccabe."

When executed, flake8 will scan through your Python code and check it against specific metrics, such as style conventions and structural problems commonly found in Python code. It will also look for syntax errors, missing imports, undefined variables, unused imports, and more.

Each different issue that is found will be reported to the user alongside an error message and specific line numbers where the issue occurs. This makes it easy to identify and fix problems within your code.

Overall, flake8 is an essential tool for programmers to ensure that their code is not only working correctly but is also easy to read and maintain. By running flake8 on your code regularly, you can ensure that it conforms to best practices for coding and is more likely to be error-free. 

## tldr 
 
> Tool to check the style and quality of Python code.
> More information: <https://flake8.pycqa.org/>.

- Lint a file or directory recursively:

`flake8 {{path/to/file_or_directory}}`

- Lint a file or directory recursively and show the line on which each error occurred:

`flake8 --show-source {{path/to/file_or_directory}}`

- Lint a file or directory recursively and ignore a list of rules. (All available rules can be found at flake8rules.com):

`flake8 --ignore {{rule1,rule2}} {{path/to/file_or_directory}}`

- Lint a file or directory recursively but exclude files matching the given globs or substrings:

`flake8 --exclude {{substring1,glob2}} {{path/to/file_or_directory}}`
