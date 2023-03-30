# tldr 
## chatgpt 
tldr is a command-line tool that provides simplified and succinct versions of manual pages for various commands. The tool is designed to save time and provide quick access to essential information. 

When you use the command 'tldr' with the name of the command whose manual page you want to view, it displays a simplified version of the corresponding manual page that can be easily understood by beginners or those who want to quickly learn the basic usage of a command. The information provided by tldr includes examples, syntax and command options. 

For example, if you want to view the manual page for the 'ls' command using tldr, you would enter "tldr ls" in the command line, and you would be provided with a simplified version of the manual page that outlines the basic usage of the ls command, such as listing the contents of a directory, displaying files based on the date, etc. 

## tldr 
 
> Display simple help pages for command-line tools from the tldr-pages project.
> More information: <https://tldr.sh>.

- Print the tldr page for a specific command (hint: this is how you got here!):

`tldr {{command}}`

- Print the tldr page for a specific subcommand:

`tldr {{command}}-{{subcommand}}`

- Print the tldr page for a command for a specific [p]latform:

`tldr -p {{android|linux|osx|sunos|windows}} {{command}}`

- [u]pdate the local cache of tldr pages:

`tldr -u`
