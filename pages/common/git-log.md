# git log 
## chatgpt 
The `git log` command is used to display a list of all the commits made in a Git repository, along with their metadata such as the author, date, and commit message. 

The output of the `git log` command contains several columns of information, including the commit hash (a unique identifier for each commit), the author's name, email address, and the date and time the commit was made. Additionally, there is the commit message, which provides a brief description of the changes made in that particular commit.

By default, the `git log` command displays the commits in reverse chronological order, with the most recent commit showing up first. This can be changed with various options, such as `--reverse` to display the commits in chronological order, or `--since` and `--until` to display commits within a specific time range.

In summary, the `git log` command is a useful tool for tracking changes made to a Git repository, allowing developers to study the history of a project and review past updates. 

## tldr 
 
> Show a history of commits.
> More information: <https://git-scm.com/docs/git-log>.

- Show the sequence of commits starting from the current one, in reverse chronological order of the Git repository in the current working directory:

`git log`

- Show the history of a particular file or directory, including differences:

`git log -p {{path/to/file_or_directory}}`

- Show an overview of which file(s) changed in each commit:

`git log --stat`

- Show a graph of commits in the current branch using only the first line of each commit message:

`git log --oneline --graph`

- Show a graph of all commits, tags and branches in the entire repo:

`git log --oneline --decorate --all --graph`

- Show only commits whose messages include a given string (case-insensitively):

`git log -i --grep {{search_string}}`

- Show the last N commits from a certain author:

`git log -n {{number}} --author={{author}}`

- Show commits between two dates (yyyy-mm-dd):

`git log --before="{{2017-01-29}}" --after="{{2017-01-17}}"`
