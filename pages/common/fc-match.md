# fc-match 
## chatgpt 
The `fc-match` command is used in Linux-based operating systems to find the font file that best matches a given pattern or description. The `fc-match` command works with the fontconfig library to search for the closest match to the font specified.

The syntax of the `fc-match` command is as follows:

```
fc-match [-s|-S] [-v] [-q] [-a] pattern
```

Here's an explanation of each option:

- `-s`: Only display the filename of the matched font.
- `-S`: Display a long list of font attributes for the matched font.
- `-v`: Verbose output.
- `-q`: Quiet output.
- `-a`: List all matching fonts, rather than just the best match.

The `pattern` argument can take several forms, including a font name, a font-family name, a font file name, or a fontconfig pattern specification.

Here's an example of how to use `fc-match` to find the font file for a specific font name:

```
$ fc-match "Arial"
/usr/share/fonts/truetype/msttcorefonts/Arial.ttf: "Arial" "Normal"
```

In this example, `fc-match` returns the filename of the Arial font file installed on the system.

Overall, the `fc-match` command is a useful tool for finding the font file that best matches a given pattern, and it can be used to ensure that the correct fonts are installed and available for use by various applications. 

## tldr 
 
> Match available fonts.
> More information: <https://manned.org/fc-match>.

- Return a sorted list of best matching fonts:

`fc-match -s '{{DejaVu Serif}}'`
