# figlet 
## chatgpt 
Figlet is a command-line utility tool that is used to create decorative text banners and stylized ASCII art fonts. The command "figlet" is used to invoke this tool, and it requires a message or text input as an argument.

For example, if you want to create a decorative text banner for the word "Hello," you can type the following command:

`figlet Hello`

This will generate a banner for the word "Hello" using the default ASCII art font style. However, Figlet allows you to choose from a wide range of font styles for your text banner. You can specify the font style using the "-f" option followed by the font style name. For instance, if you want to create a banner using the "slant" font style, you can use the following command:

`figlet -f slant Hello`

Additionally, you can customize the width and height of the banner using the "-w" and "-h" options, respectively. For example, to create a banner with a width of 80 columns and a height of 5 characters, you can type:

`figlet -w 80 -h 5 Hello`

Overall, the figlet command is a very useful tool for creating stylized and decorative text banners on the command-line interface. 

## tldr 
 
> Generate ASCII banners from user input.
> See also: `showfigfonts`.
> More information: <http://www.figlet.org/figlet-man.html>.

- Generate by directly inputting text:

`figlet {{input_text}}`

- Use a custom font file:

`figlet {{input_text}} -f {{path/to/font_file.flf}}`

- Use a font from the default font directory (the extension can be omitted):

`figlet {{input_text}} -f {{font_filename}}`

- Pipe command output through FIGlet:

`{{command}} | figlet`

- Show available FIGlet fonts:

`showfigfonts {{optional_string_to_display}}`
