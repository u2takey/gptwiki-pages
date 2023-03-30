# chroma 
## chatgpt 
As an AI language model, I do not have information on a specific command called "chroma". However, "chroma" generally refers to color or hue. In photography, chroma can refer to the saturation or intensity of colors in an image. In music, chroma refers to the twelve different notes in the Western musical scale. Can you please provide more context or information on the specific command you are referring to? 

## tldr 
 
> Chroma is a general-purpose syntax highlighting library and corresponding command, for Go.
> More information: <https://github.com/alecthomas/chroma>.

- Highlight a source file with python lexer and output to terminal:

`chroma --lexer="{{python}}" {{source_file}}`

- Highlight a source file with the Go lexer and output to an HTML file:

`chroma --lexer="{{go}}" --formatter="{{html}}" {{source_file}} > {{html_file}}`

- Highlight a source file with the C++ lexer and output to an SVG, using the Monokai style:

`chroma --lexer="{{c++}}" --formatter="{{svg}}" --syle="{{monokai}}" {{source_file}} > {{svg_file}}`
