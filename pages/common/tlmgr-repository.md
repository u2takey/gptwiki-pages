# tlmgr repository 
## chatgpt 
The command "tlmgr repository" is used in the TeX Live package manager to display the current configuration of the repositories where packages are downloaded and installed from.

When executed, the command will output the list of repositories that are currently configured in your Tex Live installation. By default, only the official TeX Live repository is included in the configuration. 

You can use this command to check if any additional repositories have been added, or to configure new repositories for your TeX Live installation.

The output of the command will be a list of all the repositories, showing the name of each repository, its type (e.g. CTAN or local), and its URL or path. The information can help you in selecting the appropriate repositories for your needs.

For example, if you are setting up a local repository for your organization, you can use the tlmgr repository command to confirm that the path to the local repository is correctly configured in TeX Live. 

## tldr 
 
> Manage repositories of a TeX Live installation.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- List all configured repositories and their tags (if set):

`tlmgr repository list`

- List all packages available in a specific repository:

`tlmgr repository list {{path|url|tag}}`

- Add a new repository with a specific tag (the tag is not required):

`sudo tlmgr repository add {{path|url}} {{tag}}`

- Remove a specific repository:

`sudo tlmgr repository remove {{path|url|tag}}`

- Set a new list of repositories, overwriting the previous list:

`sudo tlmgr repository set {{path|url|tag}}#{{tag}} {{path|url|tag}}#{{tag}} {{...}}`

- Show the verification status of all configured repositories:

`tlmgr repository status`
