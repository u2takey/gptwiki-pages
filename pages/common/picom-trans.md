# picom-trans 
## chatgpt 
I'm sorry, but as an AI language model, I'm not sure what specific command you are referring to. Can you please provide more context or details so I can better understand and explain it to you? 

## tldr 
 
> Set the window opacity for the `picom` window compositor.
> More information: <https://github.com/yshui/picom>.

- Set the currently focused window opacity to a specific percentage:

`picom-trans --current --opacity {{90}}`

- Set the opacity of a window with a specific name:

`picom-trans --name {{Firefox}} --opacity {{90}}`

- Set the opacity of a specific window selected via mouse cursor:

`picom-trans --select --opacity {{90}}`

- Toggle the opacity of a specific window:

`picom-trans --name {{Firefox}} --toggle`
