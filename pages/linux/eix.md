# eix 
## chatgpt 
eix is a command-line utility used in Linux-based operating systems that allows users to search for software packages in Gentoo Linux. The command scans through the package database to find matching search terms and returns a list of matching packages with brief descriptions, along with any relevant keywords that are associated with them.

When executed, eix provides a searchable interface with various sorting and filtering options that allow users to narrow down their searches based on a variety of different criteria such as package name, package description, license type, maintainers, and more.

Overall, the eix command is a useful tool for Gentoo Linux users who need to quickly search for software packages and stay up-to-date on the latest updates and releases in the package database. 

## tldr 
 
> Utilities for searching local Gentoo packages.
> Update local package cache using `eix-update`.
> More information: <https://wiki.gentoo.org/wiki/Eix>.

- Search for a package:

`eix {{package_name}}`

- Search for installed packages:

`eix --installed {{package_name}}`

- Search in package descriptions:

`eix --description "{{description}}"`

- Search by package license:

`eix --license {{license}}`

- Exclude results from search:

`eix --not --license {{license}}`
