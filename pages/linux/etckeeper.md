# etckeeper 
## chatgpt 
Etckeeper is a command-line utility that helps in tracking changes made to the /etc/ directory in Unix and Linux operating systems. The /etc/ directory contains configuration files for the system and applications, and any changes made can have a significant impact on the system's functioning. 

Etckeeper works by integrating with a version control system, such as Git, Mercurial, or Bazaar. It automatically creates a repository in the /etc/ directory and commits any changes made to the configuration files. 

You can use the etckeeper command to perform various actions. Here are some of the most commonly used commands:

- `etckeeper init` - This command initializes etckeeper in the /etc/ directory by creating a repository and committing the existing configuration files to it.
- `etckeeper commit "commit message"` - This command commits any changes made to the configuration files to the etckeeper repository with a commit message. You can use this command whenever you make changes to the /etc/ directory.
- `etckeeper show` - This command shows the changes made to the /etc/ directory since the last commit.
- `etckeeper diff` - This command shows the differences between the current configuration files and the last committed version.
- `etckeeper vcs <command>` - This command allows you to run arbitrary version control system commands on the etckeeper repository. For example, `etckeeper vcs status` shows the status of the repository.

Using etckeeper can help you keep track of changes made to the /etc/ directory, which can make it easier to troubleshoot issues and roll back changes if necessary. 

## tldr 
 
> Track system configuration files in Git.
> More information: <http://etckeeper.branchable.com/>.

- Set up a Git repo and perform various setup tasks (run from `/etc`):

`sudo etckeeper init`

- Commit all changes in `/etc`:

`sudo etckeeper commit {{message}}`

- Run arbitrary Git commands:

`sudo etckeeper vcs {{status}}`

- Check if there are uncommitted changes (only returns an exit code):

`sudo etckeeper unclean`

- Destroy existing repo and stop tracking changes:

`sudo etckeeper uninit`
