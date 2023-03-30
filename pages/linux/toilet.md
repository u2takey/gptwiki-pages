# toilet 
## chatgpt 
The `toilet` command is a Linux utility that is used to create large, stylized text banners on the command line. The command can be used to create ASCII art, colorized text, and various formatting options. It is often used by users who want to create eye-catching headers for their documents, blog posts or software documentation.

By default, the `toilet` command takes a `text` argument, which represents the message that needs to be stylized. For example, the following command:

```
toilet "Hello, World"
```

will display the message "Hello, World" in a large stylized font, adding some color to it. The result of the command is an ASCII art that will look like this:

```
   _   _      _ _
 _| |_| | ___| | |
|_   _| |/ _ \ | |
  |_| |_|\___/_|_|

```

In addition to this basic functionality, the `toilet` command has several options that can be used to change the style and appearance of the text banner. Some of these options include:

- `-f` (or `--font`): allows users to specify a custom .tlf font file to be used while generating the text banner.
- `-F`: enables "figlet" compatibility mode, which makes it compatible with the `figlet` font files.
- `-Ff`: allows users to specify a custom ".flf" figlet font file to be used.
- `-W`: defines the output width for the generated text banner.
- `-w`: allows users to specify the width of the text column that the text banner will occupy.
- `-S`: defines the size of the text banner.
- `-t`: enables the use of colored text.
- `-T`: enables color with 256-color mode.

The `toilet` command can be used for many types of applications, from creating an eye-catching header for a software documentation to generating unique titles or headlines for blog posts or social media pages. Its use is not limited to developers and can be used by anyone who wants to add some personality to their work. 

## tldr 
 
> A tool to display ASCII-art fonts.
> More information: <http://caca.zoy.org/wiki/toilet>.

- Generate ASCII art for a given text:

`toilet {{input_text}}`

- Generate ASCII art using a custom font file:

`toilet {{input_text}} -f {{font_filename}}`

- Generate ASCII art using a filter:

`toilet {{input_text}} --filter {{filter_name}}`

- Show available toilet filters:

`toilet --filter list `
