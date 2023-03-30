# xeyes 
## chatgpt 
The "xeyes" command is a graphical application that creates a pair of animated eyes that follow the movement of the mouse pointer on the screen. This command is generally used for fun and entertainment, as it does not serve any specific purpose other than demonstrating the capabilities of X Window System or providing visual amusement to the user. 

The eyes are created using a basic graphical algorithm that utilizes the mouse pointer coordinates to calculate the position of the eyes on the screen. The eyes are drawn as a black circle with a smaller white circle inside, giving the illusion of a realistic iris and pupil. The eyes move and follow the mouse pointer by using the information from the mouse pointer location to adjust the position of the eyes accordingly.

To execute the "xeyes" command, you need to open a terminal window and type "xeyes" (without the quotes) and then press Enter. The eyes will appear on the screen and will start following the mouse pointer immediately.

In summary, the "xeyes" command is a simple graphical application that creates a pair of animated eyes that follow the mouse pointer on the screen. It is not a useful tool for productive work, but it can be a fun and entertaining graphical feature to experiment with. 

## tldr 
 
> Display eyes on the screen that follow the mouse cursor.
> More information: <https://manned.org/xeyes>.

- Launch xeyes on the local machine's default display:

`xeyes`

- Launch xeyes on a remote machine's display 0, screen 0:

`xeyes -display {{remote_host}}:{{0}}.{{0}}`
