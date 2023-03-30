# plenv 
## chatgpt 
plenv is a command used in the context of the Perl programming language. It is a utility used to manage multiple versions of Perl on a single system. 

When a Perl developer is working on multiple projects that use different versions of Perl, plenv can be used to create a separate environment for each project to ensure that the correct version of Perl is being used. 

plenv allows developers to easily switch between different versions of Perl and set a default version that will be used for new projects. 

Some common commands that can be used with plenv include: 
- plenv version: lists all installed versions of Perl
- plenv install: installs a specific version of Perl
- plenv shell: sets the environment to use a specific version of Perl within the current shell session
- plenv global: sets a default version of Perl to be used across all shell sessions

Overall, plenv is a useful tool for Perl developers who need to manage multiple versions of the language on a single system. 

## tldr 
 
> Switch between multiple versions of Perl.
> More information: <https://github.com/tokuhirom/plenv>.

- Show the currently selected Perl version and how it was selected:

`plenv version`

- List all available installed Perl versions:

`plenv versions`

- Set the global Perl version (used unless a local or shell version takes priority):

`plenv global {{version}}`

- Set the local application-specific Perl version (used in the current directory and all directories below it):

`plenv local {{version}}`

- Set the shell-specific Perl version (used for the current session only):

`plenv shell {{version}}`

- Display help:

`plenv`

- Display help for a command:

`plenv help {{command}}`
