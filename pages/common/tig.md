# tig 
## chatgpt 
The `tig` command is a textual user interface (TUI) for the Git version control system. It allows users to navigate Git repositories, review commit history, view branches, search through commit messages, and perform various other Git-related tasks.

`Tig` stands for "Text-mode Interface for Git". It is a command-line tool that runs in your terminal emulator and provides an interactive interface for accessing and interacting with Git repositories.

When you run the `tig` command, it opens a new window in your terminal emulator that displays a summary of the current repository. From there, you can use various keybindings to navigate around the repository and perform actions such as:

- Viewing commit history: You can use the up and down arrow keys to move through the list of commits, and press Enter to view the details of a specific commit.

- Viewing branches: You can press the b key to open the branches menu, which shows a list of branches in the repository. You can then select a branch to view its commit history.

- Searching through commit messages: You can press the / key to open the search menu, which allows you to search for specific keywords or phrases in commit messages.

- Performing Git operations: You can use various keybindings to perform Git operations such as committing changes, pulling changes from a remote repository, and pushing changes to a remote repository.

Overall, `tig` is a powerful tool for interacting with Git repositories in a terminal environment, providing a convenient and efficient way to visualize commit history and perform various Git-related tasks. 

## tldr 
 
> A text-mode interface for Git.
> More information: <https://github.com/jonas/tig>.

- Show the sequence of commits starting from the current one in reverse chronological order:

`tig`

- Show the history of a specific branch:

`tig {{branch}}`

- Show the history of specific files or directories:

`tig {{path1 path2 ...}}`

- Show the difference between two references (such as branches or tags):

`tig {{base_ref}}..{{compared_ref}}`

- Display commits from all branches and stashes:

`tig --all`

- Start in stash view, displaying all saved stashes:

`tig stash`
