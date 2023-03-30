# choco new 
## chatgpt 
As an AI language model, I am not entirely sure if "choco new" refers to any specific command or program. However, if we assume it to be related to Chocolatey package manager for Windows, then the command "choco new" does not exist in Chocolatey. 

If you are asking about the "choco new" command that is used to create new packages using the Chocolatey package manager, then the following details can help explain it.

The "choco new" command is a command-line utility provided by Chocolatey to create new packages. The command is used to create a new package folder structure that contains the necessary files to define a Chocolatey package. These files include *.nuspec file(s) that describe the package as well as one or more powershell scripts that are used to install, uninstall, configure the package, etc. 

The command can be used like this:

`choco new <PackageName>`

where <PackageName> is the name of the package you want to create. 

Chocolatey provides a template for creating a new package, which includes a predefined folder structure, *.nuspec file(s), and a powershell script file. The package name provided in the "choco new" command is used to create the package folder structure and other necessary files. Once created, you can edit the files as required for your package and then build the package using the "choco pack" command to create a Chocolatey package (*.nupkg) that can be installed on other machines. 

In summary, "choco new" is a command used to create a new Chocolatey package. It creates a package folder structure and other necessary files for the package and allows you to define the package details by editing these files. 

## tldr 
 
> Generate new package specification files with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-new>.

- Create a new package skeleton:

`choco new {{package_name}}`

- Create a new package with a specific version:

`choco new {{package_name}} --version {{version}}`

- Create a new package with a specific maintainer name:

`choco new {{package_name}} --maintainer {{maintainer_name}}`

- Create a new package in a custom output directory:

`choco new {{package_name}} --output-directory {{path/to/directory}}`

- Create a new package with specific 32-bit and 64-bit installer URLs:

`choco new {{package_name}} url="{{url}}" url64="{{url}}"`
