# git credential-store 
## chatgpt 
The `git credential-store` command is used in Git to tell Git to use a credential helper that stores credentials to a plain-text file on disk. 

When you run `git credential-store`, Git will create a new "credential helper" that will save your Git username and password on your local file system under `~/.git-credentials`. Then, when Git needs to authenticate with a remote Git repository that requires authentication, it will read your credentials from that file.

This can be useful if you want Git to remember your credentials for a Git repository, so that you don't need to keep entering your username and password every time you access the repository. However, note that storing passwords in plain-text files on disk is a security risk, so use this option with caution, especially when working on shared machines. 

To configure Git to use this credential helper, you can run the following command:

```
git config --global credential.helper store
```

This will add the `credential.helper` configuration with the value "store" to your global Git configuration file (usually located at `~/.gitconfig`). From this point on, Git will use the credential helper created by `git credential-store` to store and retrieve your Git credentials. 

## tldr 
 
> `git` helper to store passwords on disk.
> More information: <https://git-scm.com/docs/git-credential-store>.

- Store Git credentials in a specific file:

`git config credential.helper 'store --file={{path/to/file}}'`
