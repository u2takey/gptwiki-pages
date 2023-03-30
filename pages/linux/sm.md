# sm 
## chatgpt 
I'm sorry, I need more context to provide an accurate answer. "sm" could refer to various commands depending on the operating system and context. Can you please provide more information about the specific situation or the operating system that you are referring to? 

## tldr 
 
> Displays a short message fullscreen.
> More information: <https://github.com/nomeata/screen-message>.

- Display a message in full-screen:

`sm "{{Hello World!}}"`

- Display a message with inverted colors:

`sm -i "{{Hello World!}}"`

- Display a message with a custom foreground color:

`sm -f {{blue}} "{{Hello World!}}"`

- Display a message with a custom background color:

`sm -b {{#008888}} "{{Hello World!}}"`

- Display a message rotated 3 times (in steps of 90 degrees, counterclockwise):

`sm -r {{3}} "{{Hello World!}}"`

- Display a message using the output from another command:

`{{echo "Hello World!"}} | sm -`
