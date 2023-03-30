# debchange 
## chatgpt 
The `debchange` command is a Debian package management utility that creates a new entry in the Debian's changelog file for a given package, automatically incrementing the version number of the package.

When you run the `debchange` command, it opens up an editor that allows you to add an entry to the changelog file for the current package you are working on. The editor will already contain some template text for the changelog entry, including the package name, version number, maintainer information, and date.

You can add your own entry text to the changelog to describe the changes made to the package in this version. The `debchange` command also allows you to specify the urgency level of the entry, which will affect how quickly the package will be included in distributions.

Once you save and close the editor, the `debchange` command will automatically add the new entry to the package's changelog file, and increment the version number if necessary. This is important for keeping track of changes to the package and for ensuring that dependencies are properly handled during installation and upgrade. 

## tldr 
 
> Tool for maintenance of the debian/changelog file in a Debian source package.
> More information: <https://manpages.debian.org/debchange>.

- Add a new version for a non-maintainer upload to the changelog:

`debchange --nmu`

- Add a changelog entry to the current version:

`debchange --append`

- Add a changelog entry to close the bug with specified ID:

`debchange --closes {{bug_id}}`
