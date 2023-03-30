# tlmgr generate 
## chatgpt 
The command "tlmgr generate" is used in TeX Live Manager (tlmgr) to generate a TeX Live repository in a specific format. It is typically used by developers or maintainers who want to create custom packages or distributions based on TeX Live.

When you run the "tlmgr generate" command, the tool generates a complete set of package information. This information includes package descriptors, package documentation, and installation scripts. This information is stored in the "tlpkg" directory within the TeX Live repository.

The "tlmgr generate" command has several options that you can use to customize the repository. For example, you can specify the path to the output directory or set the distribution name. Some other options include verboseness (how much output to produce), caching directories (where files are stored), and archive mode (which generates compressed archives of each package).

One of the most common uses for "tlmgr generate" is to create a custom TeX Live distribution. You can use the tool to generate a repository with only the packages that you need for your particular project. This can help keep the distribution small and focus on the specific requirements of your project.

Overall, "tlmgr generate" is a powerful command that is used in TeX Live Manager to generate a complete set of package information for a custom TeX Live repository. 

## tldr 
 
> Remake configuration files from information stored locally.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Remake the configuration file storing into a specific location:

`tlmgr generate --dest {{output_file}}`

- Remake the configuration file using a local configuration file:

`tlmgr generate --localcfg {{local_configuration_file}}`

- Run necessary programs after rebuilding configuration files:

`tlmgr generate --rebuild-sys`
