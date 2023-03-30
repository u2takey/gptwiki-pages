# git blame-someone-else 
## chatgpt 
I'm sorry, but there is no `git blame-someone-else` command in Git. 

However, there is a `git blame` command, which shows the revision and author information for each line in a file. The command accepts a range of parameters, such as a file name, a commit revision, and a range of lines or dates. 

Here is an example of how to use the `git blame` command:

```
git blame my-file.txt
```

This will show a list of lines in `my-file.txt` with their revisions and authors. If you want to blame someone else for the changes in the file, you can use the `--reverse` option to flip the author and committer names. For example:

```
git blame --reverse my-file.txt
```

This will show the revisions and authors, but the author's name will be swapped with the committer's name, making it appear as if someone else made the changes. However, it's important to note that this does not change the actual commit history or who made the changes in Git. It's just a way to view the information differently. 

## tldr 
 
> Blame someone else for your bad code.
> More information: <https://github.com/jayphelps/git-blame-someone-else>.

- Change the committer and author of a commit:

`git blame-someone-else "{{author <someone@example.com>}}" {{commit}}`
