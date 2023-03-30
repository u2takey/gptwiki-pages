# vimdiff 
## chatgpt 
`vimdiff` is a command that invokes the Vim editor in diff mode, allowing you to compare and edit two different version of a file side by side. 

When you run the command `vimdiff file1 file2`, Vim will open two windows side by side, with the contents of `file1` displayed on the left window and the contents of `file2` displayed on the right window. 

By default, Vim will highlight the differences between the two files using color coding, making it easy to identify and navigate through changes. You can use various commands and options to navigate, edit, and save the changes. 

Some useful commands in Vimdiff include:
- `]c` and `[c`: Jump to the next and previous difference respectively
- `do` and `dp`: Choose which changes to apply or unapply
- `zo` and `zc`: Open and close folded sections of text
- `:qa` or `:wqa`: Save and quit all windows opened in Vimdiff mode

Overall, `vimdiff` is a powerful tool for comparing and merging changes in two files, commonly used in software development and collaboration workflows. 

## tldr 
 
> Open up two or more files in vim and show the differences between them.
> See also `vim`, `vimtutor`, `nvim`.
> More information: <https://www.vim.org>.

- Open two files and show the differences:

`vimdiff {{file1}} {{file2}}`

- Move the cursor to the window on the left|right:

`Ctrl + w {{h|l}}`

- Jump to the previous difference:

`[c`

- Jump to the next difference:

`]c`

- Copy the highlighted difference from the other window to the current window:

`do`

- Copy the highlighted difference from the current window to the other window:

`dp`

- Update all highlights and folds:

`:diffupdate`

- Toggle the highlighted code fold:

`za`
