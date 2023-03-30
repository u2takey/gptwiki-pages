# lerna 
## chatgpt 
Lerna is a command line tool used in managing multiple JavaScript projects within a single repository. It helps with managing the dependencies between the projects and provides tools to streamline the development workflow. 

The basic syntax for a Lerna command is:

```
lerna <command> [options]
```

The most common Lerna command is `lerna bootstrap` which installs all the dependencies for the packages and links any cross-dependencies between packages, making it easy to develop and test the projects. 

Other common commands include:

- `lerna init`: Creates a new Lerna repo by initializing a package with default settings.
- `lerna add <package> [--dev] [--exact]`: Adds a package to the root and all of the packages in the repository.
- `lerna exec <command> [args]`: Executes an arbitrary command in each package.
- `lerna run <script> [--scope=<package>]`: Runs a script in a package or all packages that contain the script in the `package.json`.
- `lerna publish`: Publishes packages that have been updated to their respective package registries.

Lerna is widely used by teams and organizations who maintain and develop multiple microservices or packages. By using Lerna, they can streamline their development and release process, maintain consistency in dependencies, and reduce the time taken to manage the projects. 

## tldr 
 
> A tool for managing JavaScript projects with multiple packages.
> More information: <https://lerna.js.org>.

- Initialize project files (`lerna.json`, `package.json`, `.git`, etc.):

`lerna init`

- Install all external dependencies of each package and symlink together local dependencies:

`lerna bootstrap`

- Run a specific script for every package that contains it in its `package.json`:

`lerna run {{script}}`

- Execute an arbitrary shell command in every package:

`lerna exec -- {{ls}}`

- Publish all packages that have changed since the last release:

`lerna publish`
