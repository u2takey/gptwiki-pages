# tmsu 
## chatgpt 
TMSU is a command-line tool that allows you to organize and tag files on your computer by creating a virtual file system. The main command for using TMSU is simply "tmsu."

Here is a breakdown of some of the basic sub-commands and options for working with TMSU:

1. "tmsu init": This command initializes a new TMSU database in the current directory.

2. "tmsu tag [file] [tag]": This command adds a tag to a file. For example, "tmsu tag document.pdf important" adds the tag "important" to the file "document.pdf."

3. "tmsu untag [file] [tag]": This command removes a tag from a file.

4. "tmsu tags [file]": This command lists all of the tags associated with a file.

5. "tmsu list [tag]": This command lists all of the files that have a particular tag. For example, "tmsu list important" will list all files that have the "important" tag.

6. "tmsu rename [tag] [newtag]": This command renames a tag. For example, "tmsu rename important urgent" will rename the "important" tag to "urgent."

7. "tmsu merge [tag1] [tag2] [newtag]": This command merges two tags into a new tag. For example, "tmsu merge important work urgent" will merge the "important" and "work" tags into a new tag called "urgent."

Overall, TMSU is a powerful tool for organizing and categorizing files on your computer based on your own tagging system. 

## tldr 
 
> Simple command-line tool for tagging files.
> More information: <https://tmsu.org>.

- Tag a specific file with multiple tags:

`tmsu tag {{path/to/file.mp3}} {{music}} {{big-jazz}} {{mp3}}`

- Tag multiple files:

`tmsu tag --tags "{{music mp3}}" {{*.mp3}}`

- List tags of specified file(s):

`tmsu tags {{*.mp3}}`

- List files with specified tag(s):

`tmsu files {{big-jazz}} {{music}}`

- List files with tags matching boolean expression:

`tmsu files "{{(year >= 1990 and year <= 2000)}} and {{grunge}}"`

- Mount tmsu virtual filesystem to an existing directory:

`tmsu mount {{path/to/directory}}`
