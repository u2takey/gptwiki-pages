# po4a-updatepo 
## chatgpt 
The "po4a-updatepo" command is used in the context of translation management for software and documentation. It is a command-line tool that updates the translation files (.po files) which are used to translate the software or documentation from the source language to multiple target languages.

The updatepo command is part of the po4a toolset, which is a set of tools for managing translations in various formats. The purpose of this command is to update the translations of the latest version of the source file in the target language translation files.

The command is used by running "po4a-updatepo" from the command line or in a script, followed by the parameters and options needed to specify the source and target files' locations.

The basic usage of the command is as follows:

```
po4a-updatepo [options] SOURCEFILE [TARGETFILE]...
```

Options:

- `-f`, `--format`: Specifies the format of the translation files (.po files) to be updated. This is often determined automatically based on the file extension, or it can be explicitly set with this option. For example, `-f po` would specify that the files are gettext message catalog files.
- `-M`, `--keep-header`: Keeps the header of the translation files.
- `-w`, `--no-wrap`: Disables the automatic wrapping of long message strings. 

Arguments:

- `SOURCEFILE`: Specifies the source file that the translation files should be updated against. The command will update all the .po files in the same directory as the source file.
- `TARGETFILE`: Specifies the target files to be updated. You can specify one or multiple target files for each execution of the command.

In summary, the po4a-updatepo command updates the translation files (.po files) with new and updated strings from the source file. The command helps streamline the translation management process by automating the updating of translations in multiple target languages. 

## tldr 
 
> Update the translation (in PO format) of a documentation.
> More information: <https://po4a.org/man/man1/po4a-updatepo.1.php>.

- Update a PO file according to the modification of its origin file:

`po4a-updatepo --format {{text}} --master {{path/to/master.txt}} --po {{path/to/result.po}}`

- Get a list of available formats:

`po4a-updatepo --help-format`

- Update several PO files according to the modification of their origin file:

`po4a-updatepo --format {{text}} --master {{path/to/master.txt}} --po {{path/to/po1.po}} --po {{path/to/po2.po}}`
