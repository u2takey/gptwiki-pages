# pipwin 
## chatgpt 
pipwin is a third-party package manager for Windows users to install and manage PyPI packages with binary extensions. Unlike pip, pipwin installs pre-built binary packages instead of building packages from source code. This saves time and prevents various errors during package installation. It uses the pip command-line tool to install and manage packages, but it downloads and installs pre-built binary distributions (.whl files) from a repository called Christoph Gohlke's Python Extension Packages for Windows.

pipwin is installed using pip:

```
pip install pipwin
```

After installation, you can run pipwin commands in the command prompt or terminal. Some of the commonly used pipwin commands include:

- list: Lists all installed packages.
- install: Installs a package with its dependencies.
- reinstall: Reinstalls a package and its dependencies.
- uninstall: Uninstalls a package.

For example, if you want to install the package numpy using pipwin, you can use the following command:

```
pipwin install numpy
```

pipwin downloads and installs the pre-built binary distribution of numpy for Windows, along with its dependencies, if any. 

## tldr 
 
> A tool to install unofficial Python package binaries on Windows.
> More information: <https://github.com/lepisma/pipwin>.

- List all available packages for download:

`pipwin list`

- Search packages:

`pipwin search {{partial_name|name}}`

- Install a package:

`pipwin install {{package_name}}`

- Uninstall a package:

`pipwin uninstall {{package_name}}`

- Download a package to a specific directory:

`pipwin download --dest {{path\to\directory}} {{package_name}}`

- Install packages according to `requirements.txt`:

`pipwin install --file {{path\to\requirements.txt}}`
