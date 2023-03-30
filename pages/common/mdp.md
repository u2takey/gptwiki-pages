# mdp 
## chatgpt 
The "mdp" command is a tool for creating and displaying beautiful markdown presentation slides. It is a command-line application that can be used to create and display presentations in a terminal or console window.

The "mdp" command is primarily used to create presentation slides from markdown files. This is done by using specific markdown syntax to define the different slides within the document. Once the markdown file is created, the "mdp" command can be used to display the presentation in a terminal window.

The process of creating a presentation using "mdp" involves the following steps:

1. Install mdp: The "mdp" command needs to be installed on your system before it can be used. You can install it using your operating system's package manager or by downloading and installing it manually.

2. Create a markdown file: The markdown file should be written in a specific format that defines the different slides of the presentation. Each slide is defined using the "---" separator, and each slide can include text, images, and code snippets.

3. Display the presentation: Once the markdown file is created, you can display the presentation using the "mdp" command. This will open a terminal window displaying the first slide of the presentation.

Some useful options that can be used with the "mdp" command are:

- "-f" or "--fullscreen": Displays the presentation in fullscreen mode.
- "-t" or "--theme": Specifies the theme to be used for the presentation.
- "-c" or "--color-theme": Specifies the color theme to be used for the presentation.

In summary, the "mdp" command is a handy tool for creating and displaying beautiful presentations in a terminal window. It is particularly useful for developers and technical presenters who need to create quick and easy presentations on the go. 

## tldr 
 
> A command-line based tool to make presentations from Markdown files.
> More information: <https://github.com/visit1985/mdp>.

- Launch a presentation in the terminal from a Markdown file:

`mdp {{presentation.md}}`

- Disable fading transitions:

`mdp --nofade {{presentation.md}}`

- Invert font colors to use in terminals with light background:

`mdp --invert {{presentation.md}}`

- Disable transparency in transparent terminals:

`mdp --notrans {{presentation.md}}`
