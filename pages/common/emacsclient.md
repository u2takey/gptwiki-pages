# emacsclient 
## chatgpt 
Emacsclient is a command-line utility for interfacing with Emacs. It allows you to open files and interact with Emacs from the command line.

Here are the most common uses of emacsclient:

1. Opening files: When you want to open a file in Emacs, you can use emacsclient to open it directly from the command line. This is particularly useful when you’re already working in a terminal and don’t want to switch to a GUI application. The syntax for opening a file with emacsclient is:

```
emacsclient file.txt
```

This will open `file.txt` in Emacs, and you can start editing it right away.

2. Connecting to an existing Emacs instance: If you already have Emacs running, you can use emacsclient to connect to it and use it as your editor. The syntax for connecting to an existing Emacs instance is:

```
emacsclient -c
```

This will open a new frame in Emacs, and you can start editing files in that frame.

3. Running Emacs commands: You can also use emacsclient to run Emacs commands directly from the command line. This is particularly useful if you want to automate a repetitive task or run a command from a script. The syntax for running an Emacs command with emacsclient is:

```
emacsclient -e '(elisp-command)'
```

This will run the `elisp-command` in Emacs and return the result to the command line.

Overall, emacsclient is a useful and powerful utility for interacting with Emacs from the command line. It can simplify your workflow and make it easier to use Emacs as your primary editor. 

## tldr 
 
> Open files in an existing Emacs server.
> See also `emacs`.
> More information: <https://www.emacswiki.org/emacs/EmacsClient>.

- Open a file in an existing Emacs server (using GUI if available):

`emacsclient {{path/to/file}}`

- Open a file in console mode (without an X window):

`emacsclient --no-window-system {{path/to/file}}`

- Open a file in a new Emacs window:

`emacsclient --create-frame {{path/to/file}}`

- Evaluate a command, printing the output to `stdout`, and then quit:

`emacsclient --eval '({{command}})'`

- Specify an alternative editor in case no Emacs server is running:

`emacsclient --alternate-editor {{editor}} {{path/to/file}}`

- Stop a running Emacs server and all its instances, asking for confirmation on unsaved files:

`emacsclient --eval '(save-buffers-kill-emacs)'`
