# sonar-scanner 
## chatgpt 
`sonar-scanner` is a command-line interface tool for running SonarQube analysis on source code. SonarQube is an open-source platform for continuous inspection of code quality that allows developers to manage, measure, and analyze coding quality.

The `sonar-scanner` command is used to analyze the source code of a project and send the results to a SonarQube server for further processing. The analysis is based on a set of pre-defined rules, plugins, and metrics that evaluate the code for various quality dimensions, such as maintainability, reliability, security, and efficiency.

To use `sonar-scanner`, you need to first configure the SonarQube server and install the scanner on your machine. You can then run the `sonar-scanner` command from the command line, specifying the location of the source code to be analyzed, the SonarQube server URL, and any additional parameters, such as the project key, project name, and language.

The `sonar-scanner` command has several options, including:

- `-Dsonar.projectKey`: The unique identifier for the project in SonarQube
- `-Dsonar.projectName`: The name of the project in SonarQube
- `-Dsonar.sources`: The location of the source code to be analyzed
- `-Dsonar.host.url`: The URL of the SonarQube server
- `-Dsonar.login`: The login credentials for the SonarQube server
- `-Dsonar.password`: The password for the SonarQube server (not recommended - use an access token instead)
- `-Dsonar.language`: The programming language used in the codebase
- `-Dsonar.sourceEncoding`: The character encoding used in the source files

Once you run the `sonar-scanner` command, it will analyze the code using the pre-defined rules and metrics and provide a report on the quality of the code. The report will be available on the SonarQube server dashboard, where you can review the issues and take action to improve the coding quality of your project. 

## tldr 
 
> SonarScanner is a generic scanner for SonarQube projects that do not use build tools such as Maven, Gradle, or Ant.
> More information: <https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/>.

- Scan a project with configuration file in your project's root directory named `sonar-project.properties`:

`sonar-scanner`

- Scan a project using configuration file other than `sonar-project.properties`:

`sonar-scanner -D{{project.settings=myproject.properties}}`

- Print help information:

`sonar-scanner -h`

- Print debugging information:

`sonar-scanner -X`
