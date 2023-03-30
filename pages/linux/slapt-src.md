# slapt-src 
## chatgpt 
As an AI language model, I do not have the ability to provide personal opinion. However, I can explain to you what the command 'slapt-src' does.

'slapt-src' is a command-line tool for managing source packages on Slackware, a Linux operating system distribution. It is used to download, compile, and install packages from source code. The tool is a wrapper around other package management tools like 'pkg-config', 'autoconf', and 'automake' which are used to build packages from source.

The general syntax of the command is:

slapt-src [options] package_name

Some of the commonly used options in the command are:

- -i: Installs the specified package from source code
- -u: Updates the specified package
- -a: Builds all the available packages on the system
- -c: Cleans up the downloaded source packages

In summary, 'slapt-src' is a tool that helps in compiling and installing source packages on Slackware Linux system. It simplifies the process of building packages from source code and eliminates the need for manual configuration of build tools. 

## tldr 
 
> A utility to automate building of slackbuilds.
> SlackBuild sources need to be configured in the slapt-srcrc file.
> More information: <https://github.com/jaos/slapt-src>.

- Update the list of available slackbuilds and versions:

`slapt-src --update`

- List all available slackbuilds:

`slapt-src --list`

- Fetch, build and install the specified slackbuild(s):

`slapt-src --install {{slackbuild_name}}`

- Locate slackbuilds by their name or description:

`slapt-src --search {{search_term}}`

- Display information about a slackbuild:

`slapt-src --show {{slackbuild_name}}`
