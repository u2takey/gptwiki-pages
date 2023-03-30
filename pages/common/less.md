# less 
## chatgpt 
The `less` command is a popular pager utility for working with large files in Unix/Linux systems, and allows you to view text files and navigate through them easily. 

When you run the `less` command, it will display the contents of the file on your screen, but only one screenful at a time. You can then use the arrow keys or other navigation keys to scroll up and down through the document.

Here are some basic usage examples of the `less` command:

- To view a file, simply type `less filename` and press Enter. The contents of the file will be displayed on your screen.
- To navigate through the file, use the arrow keys or other navigation keys like PgUp, PgDn, Home, End, etc. You can also use the "/" key to search for text within the file.
- To exit the `less` command, simply press the "q" key.

Other useful features of the `less` command include the ability to display line numbers, search for regular expressions, and display multiple files at once. 

In summary, the `less` command is a very useful tool for viewing and navigating through large text files on Unix/Linux systems. 

## tldr 
 
> Open a file for interactive reading, allowing scrolling and search.
> More information: <https://greenwoodsoftware.com/less/>.

- Open a file:

`less {{source_file}}`

- Page down / up:

`<Space> (down), b (up)`

- Go to end / start of file:

`G (end), g (start)`

- Forward search for a string (press `n`/`N` to go to next/previous match):

`/{{something}}`

- Backward search for a string (press `n`/`N` to go to next/previous match):

`?{{something}}`

- Follow the output of the currently opened file:

`F`

- Open the current file in an editor:

`v`

- Exit:

`q`
