# wl-copy 
## chatgpt 
The `wl-copy` command is used in Wayland, which is a modern replacement for the traditional X11 window system used on Linux and other Unix-like operating systems.

`wl-copy` is a utility that allows you to copy text or other data to the clipboard in a Wayland session. This command is used to copy the given content to the clipboard.

For example, if you have a text file named "example.txt" that you want to copy to the clipboard using `wl-copy`, you can run the following command:

```
$ cat example.txt | wl-copy
```

This will copy the contents of the "example.txt" file to the Wayland clipboard.

`wl-copy` is often used in scripts and other automated processes where copying and pasting text or data is required. It also works well with other Wayland utilities and window managers. 

## tldr 
 
> Wayland clipboard manipulation tool.
> See also: `wl-paste`.
> More information: <https://github.com/bugaevc/wl-clipboard>.

- Copy the text to the clipboard:

`wl-copy "{{text}}"`

- Pipe the command (`ls`) output to the clipboard:

`{{ls}} | wl-copy`

- Copy for only one paste and then clear it:

`wl-copy --paste-once "{{text}}"`

- Clear the clipboard:

`wl-copy --clear`
