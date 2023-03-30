# pio test 
## chatgpt 
`pio test` is a command used to run unit tests on a PlatformIO project. 

PlatformIO is an open-source ecosystem for Internet of Things (IoT) development boards that supports a wide range of frameworks, operating systems, and programming languages. 

The `pio test` command allows developers to automate the testing of their project's functionality to ensure that everything works as expected. This command parses all test-related files such as _testcases.h, *_test*.cpp, and *.ino within the project directories and performs the test schedule. It works by compiling and linking the test code, uploading it to the appropriate device or simulator and running the tests.

The output of the `pio test` command will display the results of the tests and if any issues or failures occurred during testing. This can help developers to debug their code and fix any issues before deploying the project into production. 

Furthermore, PlatformIO provides integrated services for Continuous Integration (CI) platforms which help the developers automate the testing process using Git. Thus, developers can develop faster and with peace of mind, while making sure that their code can withstand testing and is functioning correctly. 

## tldr 
 
> Run local tests on a PlatformIO project.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_test.html>.

- Run all tests in all environments of the current PlatformIO project:

`pio test`

- Test only specific environments:

`pio test --environment {{environment1}} --environment {{environment2}}`

- Run only tests whose name matches a specific glob pattern:

`pio test --filter "{{pattern}}"`

- Ignore tests whose name matches a specific glob pattern:

`pio test --ignore "{{pattern}}"`

- Specify a port for firmware uploading:

`pio test --upload-port {{upload_port}}`

- Specify a custom configuration file for running the tests:

`pio test --project-conf {{path/to/platformio.ini}}`
