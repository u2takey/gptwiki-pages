# git delete-tag 
## chatgpt 
The command "git delete-tag" is not a valid Git command. The correct command to delete a tag in Git is "git tag -d <TAGNAME>". This command will delete the specified tag from your local repository.

Here's a breakdown of the command:

- "git tag" is the command for creating or managing tags in Git.
- "-d" is a flag that tells Git to delete the specified tag.
- "<TAGNAME>" is the name of the tag you want to delete.

When you run this command, Git will delete the specified tag from your local repository. Note that this does not delete the tag from any remote repositories or affect any commits that are already tagged with that tag. You may need to push the updated state of the repository to the remote to also delete the tag there. 

## tldr 
 
> Delete existing local and remote tags.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-delete-tag>.

- Delete a tag:

`git delete-tag {{tag_version}}`
