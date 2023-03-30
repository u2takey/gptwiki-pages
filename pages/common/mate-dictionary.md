# mate-dictionary 
## chatgpt 
The `mate-dictionary` command is used to access the dictionary application in the MATE desktop environment. 

When executed, the command will launch the dictionary application, which can be used to look up the definition of words, as well as synonyms, antonyms, and translations.

The dictionary application included with MATE is powered by the GNOME Dictionary Project, and provides access to various dictionaries in different languages. Users can choose which dictionary they want to use, and can switch between dictionaries as needed.

In order to use the `mate-dictionary` command, you must have the MATE desktop environment installed on your system. On some systems, it may be necessary to install the `mate-utils` package in order to access the dictionary application. 

## tldr 
 
> Look up words on dictionaries.
> More information: <https://manned.org/mate-dictionary>.

- Print a specific word definition:

`mate-dictionary --no-window --look-up '{{word}}'`

- Show similar words for a specific one in a new window:

`mate-dictionary --match '{{word}}'`
