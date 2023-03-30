# gum 
## chatgpt 
As an AI language model, I don't have access to the context. However, "gum" is a noun and refers to a chewy substance which is typically flavored and sweetened; it can be used to freshen breath or as a type of candy. It can also refer to a sticky substance or adhesive used for various purposes. In terms of a command, it could potentially be used to ask someone to give them a piece of gum or to request someone to clean up a sticky mess. 

## tldr 
 
> A tool for making glamorous shell scripts.
> More information: <https://github.com/charmbracelet/gum>.

- Interactively pick a specific option to print to `stdout`:

`gum choose "{{option_1}}" "{{option_2}}" "{{option_3}}"`

- Open an interactive prompt for the user to input a string with a specific placeholder:

`gum input --placeholder "{{value}}"`

- Open an interactive confirmation prompt and exit with either `0` or `1`:

`gum confirm "{{Continue?}}" --default=false --affirmative "{{Yes}}" --negative "{{No}}" {{&& echo "Yes selected" || echo "No selected"}}`

- Show a spinner while a command is taking place with text alongside:

`gum spin --spinner {{dot|line|minidot|jump|pulse|points|globe|moon|monkey|meter|hamburger}} --title "{{loading...}}" -- {{command}}`

- Format text to include emojis:

`gum format -t {{emoji}} "{{:smile: :heart: hello}}"`

- Interactively prompt for multi-line text (CTRL + D to save) and write to `data.txt`:

`gum write > {{data.txt}}`
