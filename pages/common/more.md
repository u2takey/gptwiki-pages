# more 
## chatgpt 
The "more" command is a basic text pager utility in Unix and Unix-like operating systems. The purpose of this command is to display the contents of a text file or input received through a pipeline in a manageable way by paginating the content, displaying it one screen at a time. This command is used when the content is too long to be displayed in a single screen.

Here are some of the commonly used options of the "more" command and their explanations:

1. -d: This option allows the user to specify the prompt text displayed when the user is prompted to continue to the next page. By default, the prompt is "more?"

2. -c: This option tells "more" to display the content of the file in the terminal using the full screen. This option is useful when the file has just a few lines of text.

3. -p: This option allows the user to specify the screen size. By default, "more" uses the size of the terminal window.

4. -s: This option tells the "more" command to display long stretches of blank lines as a single line. This is useful when handling large files with numerous blank lines.

5. -f: This option tells "more" to exit as soon as it encounters the end of the file instead of prompting the user to continue.

To use the "more" command, open a terminal and enter the following syntax:

more [options] file_name 

## tldr 
 
> Open a file for interactive reading, allowing scrolling and search.
> More information: <https://manned.org/more>.

- Open a file:

`more {{path/to/file}}`

- Open a file displaying from a specific line:

`more +{{line_number}} {{path/to/file}}`

- Display help:

`more --help`

- Go to the next page:

`<Space>`

- Search for a string (press `n` to go to the next match):

`/{{something}}`

- Exit:

`q`

- Display help about interactive commands:

`h`
