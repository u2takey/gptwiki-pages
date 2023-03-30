# tlmgr 
## chatgpt 
tlmgr is the command-line tool used to manage the TeX Live distribution. It allows you to install, update, and remove packages, as well as view information about packages and repositories.

Here are some common uses of the tlmgr command:

- To install a package, use the command `tlmgr install <package>` (e.g., `tlmgr install hyperref` to install the hyperref package).
- To update your TeX Live installation, use the command `tlmgr update --self --all`.
- To remove a package, use the command `tlmgr remove <package>` (e.g., `tlmgr remove tikz` to remove the TikZ package).
- To view information about a package, use the command `tlmgr info <package>` (e.g., `tlmgr info geometry` to view information about the geometry package).
- To add a new repository of packages to your TeX Live installation, use the command `tlmgr repository add <URL>` (e.g., `tlmgr repository add http://contrib.texlive.info/current/` to add the current repository of contributed packages).
- To list the packages installed on your system, use the command `tlmgr list --only-installed`.

There are many other options and commands available with tlmgr, so for more information, you can consult the TeX Live documentation or run `tlmgr --help` or `tlmgr <command> --help` for help with a specific command. 

## tldr 
 
> Manages packages and configuration options of an existing TeX Live installation.
> Some subcommands such as `tlmgr paper` have their own usage documentation.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Install a package and its dependencies:

`tlmgr install {{package}}`

- Remove a package and its dependencies:

`tlmgr remove {{package}}`

- Display information about a package:

`tlmgr info {{package}}`

- Update all packages:

`tlmgr update --all`

- Show possible updates without updating anything:

`tlmgr update --list`

- Start a GUI version of tlmgr:

`tlmgr gui`

- List all TeX Live configurations:

`tlmgr conf`
