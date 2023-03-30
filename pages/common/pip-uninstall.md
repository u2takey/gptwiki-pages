# pip uninstall 
## chatgpt 
The pip uninstall command is used to remove/uninstall a package, module or dependencies that were previously installed using pip (Python Package Installer). The command syntax is as follows:

```
pip uninstall <package-name>
```

Here, `<package-name>` refers to the name of the package you want to remove.

When you run this command, pip will remove the specified package from your Python environment, including any dependent packages that were installed along with it. Depending on the package and its dependencies, uninstalling a package might affect other packages that are also installed.

Some additional command line options available with this command are:

- `-y` or `--yes`: Automatically answer "yes" to all prompts and do not ask for confirmation before uninstalling a package.
- `--no-cache-dir`: Do not use cache directory for the package installation, which can save disk space.
- `-v` or `--verbose`: Display verbose output, including details about the package being uninstalled and any errors that occur. 

## tldr 
 
> Uninstall Python packages.
> More information: <https://pip.pypa.io>.

- Uninstall a package:

`pip uninstall {{package_name}}`

- Uninstall packages listed in a specific file:

`pip uninstall --requirement {{path/to/requirements.txt}}`

- Uninstall package without asking for confirmation:

`pip uninstall --yes {{package_name}}`
