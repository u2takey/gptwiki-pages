# einfo 
## chatgpt 
The `einfo` command is used in the Gentoo Linux operating system to display information about installed packages. Here is a detailed explanation of the command:

Syntax: `einfo [package-name]`

- `einfo` is the command itself, followed by the optional package-name argument.
- If no package-name is given, `einfo` will display general information about the Gentoo installation, including the Gentoo release, kernel version, USE flags, and more.
- If a package-name is given, `einfo` will display information about the corresponding package, including its version, description, installed files, dependencies, and more.
- `einfo` is primarily used for informational purposes, helping users to understand what packages are currently installed on their system and what they do.

Note: The `einfo` command is part of the `app-portage/gentoolkit` package, which needs to be installed before using the command. 

## tldr 
 
> Provides the number of records indexed in each field of a given database, the date of the last update of the database, and the available links from the database to other Entrez databases.
> More information: <https://www.ncbi.nlm.nih.gov/books/NBK179288/>.

- Print all database names:

`einfo -dbs`

- Print all information of the protein database in XML format:

`einfo -db {{protein}}`

- Print all fields of the nuccore database:

`einfo -db {{nuccore}} -fields`

- Print all links of the protein database:

`einfo -db {{protein}} -links`
