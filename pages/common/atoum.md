# atoum 
## chatgpt 
atoum is a modern, simple and intuitive unit testing framework for PHP that supports both traditional and behavior-driven development (BDD) methodologies. It allows you to easily write and run tests for your PHP codebase, and it can be used with various PHP versions and testing frameworks such as PHPUnit.

To use atoum, you need to install it via Composer using the following command:

composer require --dev atoum/atoum

This will install the latest version of atoum in the "dev" dependencies of your project.

Once installed, you can start writing your tests in PHP files that are located in a directory called "tests". In those files, you can define test classes that extend the atoum test class and use its assertions methods such as "assert()", "string()", "integer()" etc. to test your code.

To run your tests, you can use the atoum CLI tool that comes with your installation. You can execute it by running the following command in your terminal:

vendor/bin/atoum

This will run all the tests in the "tests" directory and output the results on the terminal. You can also pass options and arguments to the atoum command to customize its behavior and output.

Overall, atoum is a powerful and easy-to-use testing framework that can help you ensure the quality and reliability of your PHP code. 

## tldr 
 
> A simple, modern and intuitive unit testing framework for PHP.
> More information: <http://atoum.org>.

- Initialize a configuration file:

`atoum --init`

- Run all tests:

`atoum`

- Run tests using the specified configuration file:

`atoum -c {{path/to/file}}`

- Run a specific test file:

`atoum -f {{path/to/file}}`

- Run a specific directory of tests:

`atoum -d {{path/to/directory}}`

- Run all tests under a specific namespace:

`atoum -ns {{namespace}}`

- Run all tests with a specific tag:

`atoum -t {{tag}}`

- Load a custom bootstrap file before running tests:

`atoum --bootstrap-file {{path/to/file}}`
