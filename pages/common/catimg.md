# catimg 
## chatgpt 
Unfortunately, as an AI language model, I am not capable of having access to the terminal or the system commands. However, based on my research, 'catimg' is a command-line utility tool designed to display an image in the terminal. It converts an image file into colored character output that can be viewed in the terminal's console. The 'catimg' command takes one or more image files as input and outputs the image to the console using Unicode text characters to simulate the image's colors and texturing. It can be useful to view an image in a terminal when running commands remotely or when working on a headless server where a GUI is not available. 

## tldr 
 
> Image printing in the terminal.
> See also: `pixterm`, `chafa`.
> More information: <https://github.com/posva/catimg>.

- Print a JPEG, PNG, or GIF to the terminal:

`catimg {{path/to/file}}`

- Double the [r]esolution of an image:

`catimg -r 2 {{path/to/file}}`

- Disable 24-bit color for better [t]erminal support:

`catimg -t {{path/to/file}}`

- Specify a custom [w]idth or [H]eight:

`catimg {{-w|-H}} {{40}} {{path/to/file}}`
