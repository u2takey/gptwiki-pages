# tlmgr path 
## chatgpt 
The command "tlmgr path" is used in the TeX Live environment to display the current path settings for the TeX Live installation.

When executed, this command displays the values of various environment variables that are used by TeX Live, such as TEXMFHOME, TEXMFLOCAL, TEXMFVAR, TEXMFSYSVAR, TEXMFSYSCONFIG, and others. These variables are used to determine the locations of packages, configuration files, and other resources that are used by TeX Live.

By examining the output of this command, TeX Live users can determine whether their TeX Live installation is properly configured and whether it is using the expected paths for important resources.

Also, the "tlmgr path" command can be used to change the default path settings for TeX Live, if necessary. However, it is generally not recommended to modify these variables unless you are an experienced TeX Live user, as changes to these variables can have far-reaching consequences and may break other programs that depend on them. 

## tldr 
 
> Add or remove symlinks for TeX Live executables, man pages and info pages.
> This command has to be re-run for files added in the future.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Add symlinks to TeX Live files:

`sudo tlmgr path add`

- Remove symlinks to TeX Live files:

`sudo tlmgr path remove`
