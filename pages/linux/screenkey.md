# screenkey 
## chatgpt 
Screenkey is a command-line utility that displays keystrokes on the screen in real-time, making it easier for users to follow keyboard actions during demonstrations or presentations. It is a simple tool that is easy to use and is available on most Linux distributions. 

When the Screenkey command is executed in the terminal, it launches a small window that displays the current keyboard activity. As soon as you start typing, the corresponding keys appear on the Screenkey window, in the same order in which they were entered. The tool supports various keyboard shortcuts and allows users to customize the display properties to match their personal preferences.

Overall, Screenkey is a handy tool for anyone who needs to demonstrate keyboard actions during presentations or video tutorials. It is straightforward to use and does not require any technical knowledge to operate. 

## tldr 
 
> A screencast tool to display keys pressed.
> More information: <https://www.thregr.org/~wavexx/software/screenkey/>.

- Display keys which are currently being pressed on the screen:

`screenkey`

- Display keys and mouse buttons which are currently being pressed on the screen:

`screenkey --mouse`

- Launch the settings menu of screenkey:

`screenkey --show-settings`

- Launch screenkey at a specific position:

`screenkey --position {{top|center|bottom|fixed}}`

- Change the format of the key modifiers displayed on screen:

`screenkey --mods-mode {{normal|emacs|mac|win|tux}}`

- Change the appearance of screenkey:

`screenkey --bg-color "{{#a1b2c3}}" --font {{Hack}} --font-color {{yellow}} --opacity {{0.8}}`

- Drag and select a window on screen to display screenkey:

`screenkey --position fixed --geometry {{$(slop -n -f '%g')}}`
