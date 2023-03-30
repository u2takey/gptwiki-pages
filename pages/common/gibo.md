# gibo 
## chatgpt 
As an AI language model, I assume that you are referring to the `gibo` command in the context of GitHub. The `gibo` command is a command-line utility that helps GitHub users create `.gitignore` files for their repositories. 

When you execute the `gibo` command in your command line interface, you are presented with a list of commonly used templates for `.gitignore` files. These templates contain a list of files and directories that Git should ignore when tracking changes in your repository. 

The `gibo` utility is designed to make it easy to create a `.gitignore` file by providing an extensive list of templates for different programming languages, frameworks, and operating systems. To generate a `.gitignore` file, you simply need to specify the desired template for your project and run the `gibo` command. 

For example, if you are working on a Python project, you can create a `.gitignore` file that ignores common Python files and directories using the following command:

```
gibo python > .gitignore
```

This command will create a `.gitignore` file in the current directory that contains the Python template from `gibo`. 

Overall, the `gibo` command is a simple yet useful tool that can save you time and effort by automating the creation of `.gitignore` files for your GitHub repositories. 

## tldr 
 
> Fetch gitignore boilerplates.
> More information: <https://github.com/simonwhitaker/gibo>.

- List available boilerplates:

`gibo list`

- Write a boilerplate to `stdout`:

`gibo dump {{boilerplate}}`

- Write a boilerplate to .gitignore:

`gibo dump {{boilerplate}} >>{{.gitignore}}`

- Search for boilerplates containing a given string:

`gibo search {{string}}`

- Update available local boilerplates:

`gibo update`
