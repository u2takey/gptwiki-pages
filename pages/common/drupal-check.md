# drupal-check 
## chatgpt 
The `drupal-check` command is a tool used to check the codebase of a Drupal project for potential issues or problems. It analyzes the code in a Drupal project by looking for common coding errors, security vulnerabilities, deprecated or removed functions, and code that does not comply with Drupal coding standards. 

The `drupal-check` command is used primarily by developers and site builders who want to ensure that their Drupal project is running smoothly and that there are no errors that would cause security or performance issues.

Here is a breakdown of the `drupal-check` command:

- `drupal-check`: This is the name of the command that is being executed.
- The command is typically run from the command line or terminal, and requires installation of the `drupal-check` tool.
- Once executed, `drupal-check` searches for common coding errors, security vulnerabilities, deprecated or removed functions, and code that does not comply with Drupal coding standards.
- `drupal-check` outputs a list of any issues found during its analysis, including details about the issue and the file or files where the issue is present.
- The developer or site builder can then review the results and make any necessary changes to the code to resolve any issues identified by `drupal-check`.

In summary, `drupal-check` is a useful tool for ensuring that a Drupal project is free of errors and compliant with established Drupal standards. It helps developers and site builders to identify issues early on in the development process and make the necessary corrections to improve the performance and security of their projects. 

## tldr 
 
> Check Drupal PHP code for deprecations.
> More information: <https://github.com/mglaman/drupal-check>.

- Check the code in a specific directory for deprecations:

`drupal-check {{path/to/directory}}`

- Check the code excluding a comma-separated list of directories:

`drupal-check --exclude-dir {{path/to/excluded_directory}},{{path/to/excluded_files/*.php}} {{path/to/directory}}`

- Don't show a progress bar:

`drupal-check --no-progress {{path/to/directory}}`

- Perform static analysis to detect bad coding practices:

`drupal-check --analysis {{path/to/directory}}`
