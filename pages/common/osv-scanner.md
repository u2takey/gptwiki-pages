# osv-scanner 
## chatgpt 
As an AI language model, I do not know of any specific tool called "osv-scanner", but I can provide a general explanation of how a command works:

In general, a command is an instruction given to a computer program to perform a specific task. The osv-scanner command likely refers to a security scanner tool specifically designed for the OSV (Open Source Vulnerabilities) database. This tool scans the software components of an application or system to identify vulnerabilities and security issues present in the OSV database. 

The command may have various options and flags for customizing the scan criteria, such as specifying the directory or specific files to be scanned. Once the scan is complete, the OSV scanner generates a report outlining the potential vulnerabilities and risks it has identified within the system or application.

Overall, the osv-scanner command is likely used for evaluating the security of open source software components used within a specific project or environment to ensure that all known vulnerabilities and risks are addressed proactively. 

## tldr 
 
> Scan various mediums for dependencies and matches them against the OSV database.
> More information: <https://osv.dev/about>.

- Scan a docker image:

`osv-scanner -D {{docker_image_name}}`

- Scan a package lockfile:

`osv-scanner -L {{path/to/lockfile}}`

- Scan an SBOM file:

`osv-scanner -S {{path/to/sbom_file}}`

- Scan multiple directories recursively:

`osv-scanner -r {{directory1 directory2 ...}}`

- Skip scanning git repositories:

`osv-scanner --skip-git {{-r|-D}} {{target}}`

- Output result in JSON format:

`osv-scanner --json {{-D|-L|-S|-r}} {{target}}`
