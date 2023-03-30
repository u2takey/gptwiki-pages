# tlmgr info 
## chatgpt 
The `tlmgr info` command is a command used in TeX Live Manager (tlmgr) to display detailed information about a package or bundle. When executed, the command presents a summary of the package, including its name, version, location on the TeX Live repository, and its short description.

Here are some of the key components of the `tlmgr info` command:

- `tlmgr`: this is the TeX Live Manager utility that allows you to install, update, and manage packages and bundles within a TeX Live distribution.

- `info`: this is a subcommand that tells `tlmgr` to display information about a package or bundle.

- Package or bundle name: this is the name of the package or bundle that you want to inspect. For example, if you want to see information about the `amsfonts` package, you would type `tlmgr info amsfonts`.

- Output format: by default, `tlmgr info` produces output in a human-readable format. However, you can also request JSON-formatted output by using the `--json` option.

The `tlmgr info` command is a useful tool for obtaining information about a specific package or bundle, which can help you determine if it is the right tool for your needs. 

## tldr 
 
> Show information about TeX Live packages.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- List all available TeX Live packages, prefexing installed ones with `i`:

`tlmgr info`

- List all available collections:

`tlmgr info collections`

- List all available schemes:

`tlmgr info scheme`

- Show information about a specific package:

`tlmgr info {{package_name}}`

- List all files contained in a specific package:

`tlmgr info {{package_name}} --list`

- List all installed packages:

`tlmgr info --only-installed`

- Show only specific information about a package:

`tlmgr info {{package_name}} --data "{{name}},{{category}},{{installed}},{{size}},{{depends}},..."`

- Print all available packages as JSON encoded array:

`tlmgr info --json`
