# pastel 
## chatgpt 
The `pastel` command is a tool used for generating and manipulating colors in the Terminal. It provides a simple and intuitive way to work with colors, allowing you to create, modify, and view colors quickly and easily.

When you run the `pastel` command in your Terminal, you will be presented with a list of options and subcommands that can be used to perform various color-related tasks. Some of the main subcommands include:

- `palette` - this subcommand allows you to view and modify the current color palette used by `pastel`. You can add, remove, or modify colors in the palette to suit your needs.

- `generate` - this subcommand allows you to generate random colors or color schemes based on various parameters, such as hue, saturation, and brightness.

- `blend` - this subcommand allows you to mix two or more colors together to create a new color. You can specify the amount of each color to use in the mix, as well as the blending mode to be used.

- `convert` - this subcommand allows you to convert colors between different formats, such as hex, RGB, and HSL.

Overall, `pastel` is a powerful and versatile tool for working with colors in the Terminal, whether you're a designer, developer, or just someone who wants to add some color to their Terminal prompt. 

## tldr 
 
> Generate, analyze, convert and manipulate colors.
> More information: <https://github.com/sharkdp/pastel>.

- Convert colors from one format to another. Here from RGB to HSL:

`pastel format {{hsl}} {{ff8000}}`

- Show and analyze colors on the terminal:

`pastel color "{{rgb(255,50,127)}}"`

- Pick a color from somewhere on the screen:

`pastel pick`

- Generate a set of N visually distinct colors:

`pastel distinct {{8}}`

- Get a list of all X11 / CSS color names:

`pastel list`
