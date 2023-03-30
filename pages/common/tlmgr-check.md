# tlmgr check 
## chatgpt 
The command "tlmgr check" is used in the TeX Live distribution system to verify the integrity of the installed packages, their dependencies, and other supporting files. When the command is executed, TeX Live Manager (tlmgr) scans the local installation and checks for any inconsistencies such as missing or broken files, outdated packages, or conflicts with other installed packages. 

If any issues are found, tlmgr provides appropriate suggestions to fix the inconsistencies or conflicts. The command also generates a report on the current installation status of TeX Live packages and their associated files.

Overall, the "tlmgr check" command helps ensure the stability and consistency of the TeX Live installation and prevent possible errors or crashes when working with TeX documents. This command is recommended to be run periodically to ensure that the installed packages are up-to-date, and no critical issues are present. 

## tldr 
 
> Check the consistency of a TeX Live installation.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Check the consistency of the whole TeX Live installation:

`tlmgr check all`

- Check the consistency of the whole TeX Live information in verbose mode:

`tlmgr check all -v`

- Check for missing dependencies:

`tlmgr check depends`

- Check if all TeX Live executables are present:

`tlmgr check executes`

- Check if all files listed in the local TLPDB are present:

`tlmgr check files`

- Check for duplicate filenames in the runfiles sections:

`tlmgr check runfiles`
