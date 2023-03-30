# kahlan 
## chatgpt 
Kahlan is a command-line tool for testing PHP applications. It provides a behavior-driven development (BDD) style of testing, allowing you to write tests using natural language syntax. This makes it easier to understand what the tests are doing and how the application should behave.

When you run the "kahlan" command, it will search for test files in the "spec" directory of your PHP application. It will then execute the tests and report any failures or errors.

Kahlan provides a range of features to help you write effective tests, such as mocking and stubbing, spies, and coverage reporting. You can also configure it to work with different testing frameworks or integrate it with other tools in your workflow.

Overall, the "kahlan" command is a powerful tool for PHP developers who want to ensure their applications are functioning as intended and catch any potential issues before they cause problems. 

## tldr 
 
> A unit and Behaviour Driven Development test framework for PHP.
> More information: <https://kahlan.github.io>.

- Run all specifications in the "spec" directory:

`kahlan`

- Run specifications using a specific configuration file:

`kahlan --config={{path/to/configuration_file}}`

- Run specifications and output using a reporter:

`kahlan --reporter={{dot|bar|json|tap|verbose}}`

- Run specifications with code coverage (detail can be between 0 and 4):

`kahlan --coverage={{detail_level}}`
