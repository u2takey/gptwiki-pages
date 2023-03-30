# rpmspec 
## chatgpt 
The `rpmspec` command is a tool used in Linux-based operating systems to generate and manipulate `.spec` files, which are used to build RPM packages. Here are some of the main features and options of the `rpmspec` command:

- `rpmspec -q`: This option queries an RPM spec file and reports its attributes, including its name, version, release, summary, description, and list of files included in the package.
- `rpmspec -bi`: This option generates a binary RPM package from a spec file.
- `rpmspec -bp`: This option extracts the sources needed to build the package from the source RPM file.
- `rpmspec -bc`: This option builds a package from the extracted sources, without doing a full build and install.
- `rpmspec -ba`: This option builds the package from the sources and installs it on the local system, creating a binary RPM package.
- `rpmspec -bs`: This option builds a source RPM package, which contains the sources but not the binary files. This is useful for distributing source code.
- `rpmspec -qf <filename>`: This option queries the RPM package that contains the specified file, reporting its attributes, including its name, version, release, and summary.

Overall, the `rpmspec` command is a powerful tool for managing and building RPM packages, and it is commonly used by developers and system administrators who work with Linux-based systems. 

## tldr 
 
> Query a RPM spec file.
> More information: <https://manned.org/rpmspec>.

- List binary packages which would be generated from a rpm spec file:

`rpmspec --query {{path/to/rpm.spec}}`

- List all options for `--queryformat`:

`rpmspec --querytags`

- Get summary information for single binary packages generated from a rpm spec file:

`rpmspec --query --queryformat "{{%{name}: %{summary}\n}}" {{path/to/rpm.spec}}`

- Get the source package which would be generated from a rpm spec file:

`rpmspec --query --srpm {{path/to/rpm.spec}}`

- Parse a rpm spec file to `stdout`:

`rpmspec --parse {{path/to/rpm.spec}}`
