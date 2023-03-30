# hadolint 
## chatgpt 
Hadolint is a command-line tool used for analyzing Dockerfiles and reporting potential issues that could lead to security vulnerabilities, bugs, or inefficiencies. It uses the Docker API and best practices to validate Dockerfiles and provide feedback to improve their overall quality.

The command "hadolint" is used to execute this tool on a Dockerfile. When executed, it will scan the Dockerfile for potential issues and report any found to the user. The command can be run with different options to fine-tune the output and the level of scrutiny applied to the Dockerfile.

Some common options that can be passed to the "hadolint" command include:

- "-f": specifies the file to analyze (e.g., "hadolint -f Dockerfile" will analyze the Dockerfile in the current directory).
- "-c": specifies the configuration file with additional rules or exclusions (e.g., "hadolint -c myconfig.yaml -f Dockerfile").
- "-v": sets the verbosity level of the output (e.g., "hadolint -v error -f Dockerfile" will only print errors).
- "-D": enables the debug mode to display additional information about the Dockerfile being analyzed (e.g., "hadolint -D -f Dockerfile").

After running the "hadolint" command, the output will display a summary of the found issues, including the line number and description of the problem. It is then up to the user to review and fix the issues identified by the tool. 

## tldr 
 
> Dockerfile linter.
> More information: <https://github.com/hadolint/hadolint>.

- Lint a Dockerfile:

`hadolint {{path/to/Dockerfile}}`

- Lint a Dockerfile, displaying the output in JSON format:

`hadolint --format {{json}} {{path/to/Dockerfile}}`

- Lint a Dockerfile, displaying the output in a specific format:

`hadolint --format {{tty|json|checkstyle|codeclimate|codacy}} {{path/to/Dockerfile}}`

- Lint a Dockerfile ignoring specific rules:

`hadolint --ignore {{DL3006}} --ignore {{DL3008}} {{path/to/Dockerfile}}`

- Lint multiple Dockerfiles using specific trusted registries:

`hadolint --trusted-registry {{docker.io}} --trusted-registry {{example.com}}:{{5000}} {{path/to/Dockerfile}} {{path/to/another/Dockerfile}}`
