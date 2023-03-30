# check-language-support 
## chatgpt 
The `check-language-support` command is a Linux command that checks for the availability of language support packages installed on the system. 

When executed, the command scans the system and identifies the languages that are supported. It checks for the installed language packages and reports which ones are missing. The command is mainly used to verify that the required language support packages are present on the system to run applications in different languages.

The output of the command displays a list of language codes that are supported on the system, along with the status of the packages for each language. The status values could be `install`, `remove`, or `not-installed`, indicating if the package is installed, can be removed, or is not present on the system.

For example, a sample output of the `check-language-support` command may look like this:

```
$ check-language-support
en: Install
en_AU: Install
en_CA: Install
en_GB: Install
zh_CN: Not installed
zh_TW: Not installed
```

In this output, the system supports English, Australian English, Canadian English, and British English, and all of them are installed. However, Chinese languages (Simplified and Traditional) are not installed on the system. The output helps the user to determine which support packages are needed for a particular language to ensure that applications in that language run without issues. 

## tldr 
 
> Display a list of missing language packages on Ubuntu.
> More information: <https://manpages.ubuntu.com/manpages/latest/man1/check-language-support.html>.

- Display a list of missing language packages based on installed software and enabled locales:

`check-language-support`

- List packages for a specific locale:

`check-language-support --language {{en}}`

- Display installed packages as well as missing ones:

`check-language-support --show-installed`
