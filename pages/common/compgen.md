# compgen 
## chatgpt 
compgen is a built-in command in Bash that is used to generate a list of possible completions of a given command or alias.

Syntax: compgen [-abcdefgjksuv] [-o option] [-A action] [-G globpat] [-W wordlist] [-F function] [-C command] [-X filterpat] [-P prefix] [-S suffix] [word]

Options:
-abcdefgjksuv: These are different options that can be used to modify the behavior of the compgen command.
-o option: Specifies the type of completions to generate. Some common options are: file (for filenames), alias (for aliases), function (for function names), and variable (for variable names).
-A action: Specifies an action to be taken on each completion. The default action is to simply print it out. Other actions include adding a prefix or suffix to the completion.
-G globpat: Specifies a glob pattern to filter out some completions.
-W wordlist: Specifies a list of words to use for completion. This is often used in combination with the -o option.
-F function: Specifies a function to use for generating completions.
-C command: Specifies a command to use for generating completions.
-X filterpat: Specifies a regular expression pattern to filter out some completions.
-P prefix: Specifies a prefix to add to each completion.
-S suffix: Specifies a suffix to add to each completion.

Overall, compgen is a powerful command that allows users to quickly generate a list of possible completions for a given context. It is especially useful when combined with other commands and options, such as the -o option or the -W wordlist option. 

## tldr 
 
> A built-in command for auto-completion in Bash, which is called on pressing TAB key twice.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#index-compgen>.

- List all commands that you could run:

`compgen -c`

- List all aliases:

`compgen -a`

- List all functions that you could run:

`compgen -A function`

- Show shell reserved keywords:

`compgen -k`

- See all available commands/aliases starting with 'ls':

`compgen -ac {{ls}}`
