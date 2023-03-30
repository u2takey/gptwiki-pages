# git mailinfo 
## chatgpt 
The "git mailinfo" command is used in Git to extract information about email messages from patch files. It is typically used when importing changes from email-based workflows or email-based patch review systems.

When the "git mailinfo" command is executed, Git reads the patch file and extracts information such as the sender, recipient, subject, date, and body from the email message contained in the patch. This information is then passed on to Git's patch application tools, which can apply the patches to the relevant files and branches in the repository.

The "git mailinfo" command can also be used in combination with other Git commands, such as "git am" or "git apply", to automate the application of patches from email-based workflows.

Overall, the "git mailinfo" command is an essential tool for working with email-based workflows and patch review systems in Git. It can help to streamline the process of applying patches and ensure that patches are applied correctly and consistently. 

## tldr 
 
> Extract patch and authorship information from a single email message.
> More information: <https://git-scm.com/docs/git-mailinfo>.

- Extract the patch and author data from an email message:

`git mailinfo {{message|patch}}`

- Extract but remove leading and trailing whitespace:

`git mailinfo -k {{message|patch}}`

- Remove everything from the body before a scissors line (e.g. "-->* --") and retrieve the message or patch:

`git mailinfo --scissors {{message|patch}}`
