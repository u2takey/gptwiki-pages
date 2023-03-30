# manpath 
## chatgpt 
The command "manpath" is a Linux command that is used to display the current search path for manual pages. It shows the directories where man pages are located.

When a user types a command followed by the "man" keyword in the terminal, the man pages will be displayed. These pages contain documentation about a command or utility that describes how to use it or its features. The "manpath" command locates these man pages and shows their directory paths.

The output of the "manpath" command displays the directories that are searched for manual pages. By default, these are /usr/local/man, /usr/share/man, and /usr/man. However, the search path can be customized by editing the MANPATH environment variable.

In summary, "manpath" is a helpful command for locating and managing the search path for manual pages on a Linux system. 

## tldr 
 
> Determine the search path for manual pages.
> More information: <https://manned.org/manpath>.

- Display the search path used to find man pages:

`manpath`

- Show the entire global manpath:

`manpath --global`
