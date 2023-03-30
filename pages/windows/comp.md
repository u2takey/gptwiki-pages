# comp 
## chatgpt 
The comp command is a Windows command that compares the contents of two files or sets of files. When executed, it compares the contents of two files and reports if they are different, and if so, where the differences occur.

Syntax:
comp [options] file1 file2

Parameters:
- [options]: specifies the command line options to use. There are several switches for this command such as /A, /B, /C, /D, /E, /L etc.
- file1: specifies the first file to compare.
- file2: specifies the second file to compare.

Switches:
- /A: specifies that COMP should use ASCII mode for comparing files.
- /B: specifies that COMP should perform a binary comparison of the files.
- /C: specifies that COMP should be case sensitive when comparing files.
- /D: specifies that COMP should display differences in decimal format.
- /L: specifies that COMP should perform a comparison of files in a case-insensitive manner.
- /N: specifies that COMP should not check for the existence of a file before comparing it.
- /U: specifies that COMP should perform a comparison of files in a case-sensitive manner.
- /W: specifies that COMP should ignore all spaces and tabs when comparing files.

Examples:
1. To compare two text files and display the differences:
comp file1.txt file2.txt

2. To compare two binary files and display the differences:
comp /B file1.bin file2.bin

3. To compare two files and display the differences in decimal format:
comp /D file1.txt file2.txt

In summary, the comp command is used in Windows to compare the contents of two files or sets of files and report any differences found between them. The output of the command shows the location of the differences and which line number they occur on. 

## tldr 
 
> Compare the contents of two files or sets of files.
> Use wildcards (*) to compare sets of files.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/comp>.

- Compare files interactively:

`comp`

- Compare two specified files:

`comp {{path\to\file1}} {{path\to\file2}}`

- Compare two sets of files:

`comp {{path\to\directory1}}\* {{path\to\directory2}}\*`

- Display differences in decimal format:

`comp /d {{path\to\file1}} {{path\to\file2}}`

- Display differences in ASCII format:

`comp /a {{path\to\file1}} {{path\to\file2}}`

- Display line numbers for differences:

`comp /l {{path\to\file1}} {{path\to\file2}}`

- Compare files case-insensitively:

`comp /c {{path\to\file1}} {{path\to\file2}}`

- Compare only the first 5 lines of each file:

`comp /n={{5}} {{path\to\file1}} {{path\to\file2}}`
