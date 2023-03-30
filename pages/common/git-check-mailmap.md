# git check-mailmap 
## chatgpt 
The command "git check-mailmap" checks whether email addresses or usernames have been mapped in the ".mailmap" file of a Git repository.

The ".mailmap" file is a text file that can contain information about aliases and alternative email addresses. The file can be used to clarify a contributor's identity by listing all the various email addresses and usernames they may have used when making contributions to the repository.

When the "git check-mailmap" command is executed, Git scans through the ".mailmap" file, and if any mappings are found, it displays them to the user. The mappings are displayed in the format of "canonical-name <email>" for each username or email address.

This command is useful when working with a repository that has contributions from multiple individuals who have used different email addresses or usernames. By using the ".mailmap" file, the contributors' identities can be consolidated and made consistent. It can also be helpful in resolving merge conflicts and tracking down individual contributions to the repository. 

## tldr 
 
> Show canonical names and email addresses of contacts.
> More information: <https://git-scm.com/docs/git-check-mailmap>.

- Look up the canonical name associated with an email address:

`git check-mailmap "<{{email@example.com}}>"`
