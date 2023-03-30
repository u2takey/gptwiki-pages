# doctum 
## chatgpt 
Unfortunately, as an AI language model, I do not have access to the specific context of your question. However, I can tell you that Doctum is a tool for generating API documentation. It's commonly used with PHP and is similar to tools like Swagger or Sphinx. 

In general, the `doctum` command is used to generate documentation for a codebase. It takes in certain inputs like the location of the codebase, the output location for the documentation, and any configuration options, and then generates the documentation accordingly. 

Some common options for the `doctum` command include:

- `--project`: the directory containing the codebase to generate documentation for
- `--output-dir`: the directory where the generated documentation should be placed
- `--config-file`: the path to a configuration file specifying options for the generation process
- `--force`: overwrite any existing documentation in the output directory
- `--quiet`: suppress all output except for errors 

Overall, the specific usage of the `doctum` command will vary depending on the codebase being documented, the desired output format, and any other configuration options. 

## tldr 
 
> A PHP API documentation generator.
> More information: <https://github.com/code-lts/doctum>.

- Parse a project:

`doctum parse`

- Render a project:

`doctum render`

- Parse then render a project:

`doctum update`

- Parse and render only a specific version of a project:

`doctum update --only-version={{version}}`

- Parse and render a project using a specific configuration:

`doctum update {{path/to/config.php}}`
