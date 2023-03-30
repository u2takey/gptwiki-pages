# hg 
## chatgpt 
The command "hg" is used to interact with the Mercurial version control system. Mercurial is a distributed version control system that allows multiple developers to work on the same codebase and track changes that have been made. 

When the "hg" command is executed in the command line, it displays a list of available subcommands and options that can be used with Mercurial. The most commonly used subcommands include:

- clone: create a local copy of a remote repository
- init: create a new repository in the current directory
- add: stage changes to be committed
- commit: save changes to the repository with a commit message
- push: send changes to a remote repository
- pull: fetch changes from a remote repository
- status: show the status of files in the repository

Mercurial also allows the use of extensions, which can provide additional functionality not included in the base system. These extensions can be enabled using the "hg extname" command, where "extname" is the name of the extension.

Overall, the "hg" command is the entry point for interacting with Mercurial and managing code repositories. 

## tldr 
 
> A command-line interface for Mercurial, a distributed source control management system.
> Some subcommands such as `hg commit` have their own usage documentation.
> More information: <https://www.mercurial-scm.org>.

- Execute Mercurial command:

`hg {{command}}`

- Call general help:

`hg help`

- Call help on a command:

`hg help {{command}}`

- Check the Mercurial version:

`hg --version`
