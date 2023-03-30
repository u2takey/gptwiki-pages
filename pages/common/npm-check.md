# npm-check 
## chatgpt 
The `npm-check` command is used to check the package dependencies within a Node.js project. It is a command-line utility that helps developers keep track of out-of-date or vulnerable package versions and provides suggestions on how to update them. 

Using the `npm-check` command, a developer can see a summary of all the installed packages and their version numbers, as well as their current status: up-to-date, outdated or insecure. It also displays the latest available versions of the packages that are installed and lets developers know if there are any breaking changes or if the upgrade will require manual intervention. 

The `npm-check` command can also be used to automatically update the packages by running a command like `npm-check -u`. This will update all the packages to their latest versions, based on the information provided by `npm-check`. However, it is important to note that updating packages can sometimes cause issues, so it is recommended to use this command with caution and to assess any potential risks before updating.

In summary, `npm-check` is a useful tool for managing package dependencies in Node.js projects, and can help developers stay up-to-date with the latest package versions while ensuring security and stability. 

## tldr 
 
> Check for outdated, incorrect, and unused npm package dependencies.
> More information: <https://github.com/dylang/npm-check>.

- Display a report of outdated, incorrect, and unused dependencies:

`npm-check`

- Interactively update out-of-date packages:

`npm-check --update`

- Update everything without prompting:

`npm-check --update-all`

- Don't check for unused packages:

`npm-check --skip-unused`
