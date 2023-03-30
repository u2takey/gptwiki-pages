# pup 
## chatgpt 
As an AI language model, I should clarify that there are several commands with the keyword "pup." Therefore, I'll provide more information about the possible commands with the term "pup" and their meaning:

1. Pup (Parsing HTML at the Command Line): This command is used to extract data from HTML documents at the command line. Pup uses CSS selectors to extract the required data from an HTML document. It supports HTML5 and can handle malformed HTML.

2. Pup (Package Updater for Arch-based Linux Distributions): This command is used to update packages on Arch-based Linux distributions. It provides a simpler and friendlier interface than Pacman, the default package manager on Arch-based distributions.

3. Pup (Portable Unix Password Manager): This command is a command-line tool for managing passwords. It is written in POSIX shell and supports encryption and GPG.

4. Pup (Pager Up and Page Down): This command is used to scroll up and down the terminal output. It is used along with less command to make the scrolling more user-friendly.

Therefore, the meaning and usage of the command "pup" depend upon the context in which it is being used. 

## tldr 
 
> Command-line HTML parsing tool.
> More information: <https://github.com/ericchiang/pup>.

- Transform a raw HTML file into a cleaned, indented, and colored format:

`cat {{index.html}} | pup --color`

- Filter HTML by element tag name:

`cat {{index.html}} | pup '{{tag}}'`

- Filter HTML by id:

`cat {{index.html}} | pup '{{div#id}}'`

- Filter HTML by attribute value:

`cat {{index.html}} | pup '{{input[type="text"]}}'`

- Print all text from the filtered HTML elements and their children:

`cat {{index.html}} | pup '{{div}} text{}'`

- Print HTML as JSON:

`cat {{index.html}} | pup '{{div}} json{}'`
