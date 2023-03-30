# aspell 
## chatgpt 
`aspell` is a command-line tool used for spell-checking documents. It is used to check the spelling of words in text files, email messages, HTML and LaTeX documents, and many other formats. This tool can be used interactively or as part of a script, and it has many options and features to customize its behavior.

The basic syntax for using `aspell` is as follows:

`aspell [options] [file]`

Here, `options` are the various command-line options available for customizing the behavior of `aspell`, and `file` is the name of the file to be spell-checked. If no file is specified, `aspell` reads from standard input.

Some of the common options for `aspell` are:

- `-c`: Check spelling interactively, allowing you to choose replacements for misspelled words.
- `-a`: Check spelling non-interactively and output a list of misspelled words.
- `-l`: Set the language to use for the spell-checking.
- `-p`: Set the personal dictionary to use for user-defined words.

Overall, `aspell` is a versatile and powerful tool for spell-checking documents, and it is widely used for this purpose in many different contexts. 

## tldr 
 
> Interactive spell checker.
> More information: <http://aspell.net/>.

- Spell check a single file:

`aspell check {{path/to/file}}`

- List misspelled words from standard input:

`cat {{path/to/file}} | aspell list`

- Show available dictionary languages:

`aspell dicts`

- Run `aspell` with a different language (takes two-letter ISO 639 language code):

`aspell --lang={{cs}}`

- List misspelled words from standard input and ignore words from personal word list:

`cat {{path/to/file}} | aspell --personal={{personal-word-list.pws}} list`
