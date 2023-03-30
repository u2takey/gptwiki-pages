# git credential 
## chatgpt 
git credential is not a valid git command. 

However, git credential is a credential helper that Git can use to securely store and retrieve user credentials such as passwords, OAuth tokens, and SSH keys. This credential helper is typically used with Git over HTTPS to authenticate users with Git servers that require authentication.

To use git credential, you would typically add it to your Git configuration. This can be done by running the following command:

```
$ git config --global credential.helper <helper>
```

Replace `<helper>` with the name of the credential helper you want to use. For example, to use the default credential helper for Mac OS X, you would use:

```
$ git config --global credential.helper osxkeychain
```

Once configured, Git will automatically invoke the credential helper when needed to obtain user credentials. The credentials are then securely stored on disk or in a keychain and can be retrieved automatically by Git when requested. This eliminates the need to enter credentials every time you interact with a Git server that requires authentication. 

## tldr 
 
> Retrieve and store user credentials.
> More information: <https://git-scm.com/docs/git-credential>.

- Display credential information, retrieving the username and password from configuration files:

`echo "{{url=http://example.com}}" | git credential fill`

- Send credential information to all configured credential helpers to store for later use:

`echo "{{url=http://example.com}}" | git credential approve`

- Erase the specified credential information from all the configured credential helpers:

`echo "{{url=http://example.com}}" | git credential reject`
