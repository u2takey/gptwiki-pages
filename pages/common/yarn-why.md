# yarn-why 
## chatgpt 
`yarn-why` is not a valid command in Yarn. 

However, `yarn why <package>` is a valid command in Yarn. This command is used to show why a package is installed in your project, indicating which other packages depend on it. 

The `yarn why` command can also be used to troubleshoot dependency conflicts by showing why a specific version of a package was installed instead of another version, as well as potential resolutions to conflicts. 

For example, if we run the command `yarn why lodash` in a Yarn project, we may see something like:

```
yarn why v1.22.11
[1/4] 🤔  Why do we have the module "lodash"...?
[2/4] 🚚  Initialising dependency graph...
[3/4] 🔍  Finding dependency...
[4/4] 🚡  Calculating file sizes...
=> Found "lodash@4.17.20"
info This module exists because "axios@0.21.0" depends on it.
```

This output shows that the `lodash` module is installed in the project because it is a dependency of `axios@0.21.0`. Knowing why a package is installed can help developers understand the impact of removing or updating that package. 

## tldr 
 
> Identifies why a Yarn package has been installed.
> More information: <https://github.com/amio/yarn-why>.

- Show why a Yarn package is installed:

`yarn-why {{package_name}}`
