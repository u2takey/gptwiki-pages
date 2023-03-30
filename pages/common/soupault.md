# soupault 
## chatgpt 
Soupault is a command-line tool for static website generation. It allows users to create static websites through a configuration file and content in Markdown format. It can also be used to generate documentation or blog websites. 

Here are some basic commands and their explanations:

1. `soupault init`: This command initializes a new project with some boilerplate files and a sample configuration file. 

2. `soupault build`: This command builds the website from the source files and the configuration file. 

3. `soupault serve`: This command launches a local server that serves the website. This is useful for previewing the website before deployment. 

4. `soupault check`: This command checks for errors and inconsistencies in the configuration file and source files. 

5. `soupault update`: This command updates the soupault tool to the latest version. 

6. `soupault help`: This command displays a list of available commands and their descriptions. 

Overall, soupault is a powerful command-line tool for generating static websites with ease. Its simple configuration format and support for Markdown make it a popular choice among developers and bloggers. 

## tldr 
 
> Soupault is a static website generator based on HTML element tree rewriting.
> It can also be used as an HTML post-processor or metadata extractor.
> More information: <https://soupault.app>.

- Initialize a minimal website project in the current working directory:

`soupault --init`

- Build a website:

`soupault`

- Override default config file and directory locations:

`soupault --config {{config_path}} --site-dir {{input_dir}} --build-dir {{output_dir}}`

- Extract metadata into a JSON file without generating pages:

`soupault --index-only --dump-index-json {{path/to/file.json}}`

- Show the effective config (values from `soupault.toml` plus defaults):

`soupault --show-effective-config`
