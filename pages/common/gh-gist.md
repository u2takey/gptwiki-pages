# gh gist 
## chatgpt 
The command "gh gist" is used in the GitHub CLI tool to interact with gists. Gists are a way to share code snippets or text files with others on GitHub.

Here are some of the sub-commands that can be used with "gh gist":

- create: This sub-command is used to create a new gist. You can specify the filename, description, and content of the gist.
- edit: This sub-command is used to edit an existing gist. You can modify the filename, description, and content of the gist.
- list: This sub-command is used to list all of your gists. You can filter the list by their visibility, creation date, and other criteria.
- view: This sub-command is used to view the contents of a gist. You can specify a specific gist by its ID or URL.
- fork: This sub-command is used to create a copy of an existing gist. You can modify the copy and make it your own.

Overall, "gh gist" is a powerful command that allows developers to manage their gists directly from the command line. It can be used to create and share code snippets or text files with others on GitHub. 

## tldr 
 
> Work with GitHub Gists on the command-line.
> More information: <https://cli.github.com/manual/gh_gist>.

- Create a new Gist from a space-separated list of files:

`gh gist create {{path/to/files}}`

- Create a new Gist with a description:

`gh gist create {{path/to/file}} --desc "{{description}}"`

- Edit a Gist:

`gh gist edit {{id_or_url}}`

- List Gists owned by the currently logged in user:

`gh gist list --limit {{int}}`

- View a Gist in the default browser without rendering Markdown:

`gh gist view {{id_or_url}} --web --raw`
