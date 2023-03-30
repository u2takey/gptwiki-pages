# git bug 
## chatgpt 
I'm sorry, but "git bug" is not a valid command in Git. "git bug" is not one of the built-in Git commands, nor is it a commonly used alias or subcommand. 

It's possible that "git bug" might refer to a specific Git extension or plugin that you have installed on your system. However, without more information about the specific tool in question, it's impossible to provide a detailed explanation for the command. 

## tldr 
 
> A distributed bug tracker that uses git's internal storage, so no files are added in your project.
> You may submit your problems to the same git remote you use to interact with others, much like commits and branches.
> More information: <https://github.com/MichaelMure/git-bug/blob/master/doc/md/git-bug.md>.

- Create a new identity:

`git bug user create`

- Create a new bug:

`git bug add`

- You can push your new entry to a remote:

`git bug push`

- You can pull for updates:

`git bug pull`

- List existing bugs:

`git bug ls`

- Filter and sort bugs using a query:

`git bug ls "{{status}}:{{open}} {{sort}}:{{edit}}"`

- Search for bugs by text content:

`git bug ls "{{search_query}}" baz`
