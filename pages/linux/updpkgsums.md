# updpkgsums 
## chatgpt 
The command "updpkgsums" is used in Linux to update the checksums of a software package. It recalculates the checksum values for all the files in the package and updates them in the corresponding PKGBUILD file. 

The PKGBUILD file is a script that contains information about a software package like its version, source URL, dependencies, and other build instructions. It also contains checksums of all the files that are part of the package.

Checksums are unique signatures generated from the contents of a file. They are used to verify data integrity, detect data tampering or corruption, and ensure that the downloaded files are not compromised or malicious. When a package is updated, its checksum values may change, and hence, it becomes necessary to update the PKGBUILD file with the new checksums.

The "updpkgsums" command makes this task easy and effortless. It reads the contents of the package, recalculates the checksums of all the files, and updates the corresponding values in the PKGBUILD file. This ensures that the new package can be built and installed without any issues.

In summary, "updpkgsums" is a command-line tool that helps maintain the integrity and security of software packages in Linux by updating their checksum values in the PKGBUILD file. 

## tldr 
 
> Update the checksums of the sources in a `PKGBUILD`.
> Unless a preexisting hashing algorithm is used, SHA256 will be used.
> More information: <https://manned.org/updpkgsums>.

- Update the checksums in a `PKGBUILD`:

`updpkgsums`

- Display Version:

`updpkgsums -v`

- Display help:

`updpkgsums -h`
