# xev 
## chatgpt 
The 'xev' command is used in Linux, specifically in X Window System, to display or monitor X11 events, that is, all events that occur on an X server, including keyboard and mouse events. It opens a window where you can click, type or move the mouse and observe the detailed output of these events in the terminal it was executed. 

The output produced by the xev command includes various pieces of information on the specific event captured, such as the event type, event detail, keycode, symbol, state, mode, and others. This command can be useful for diagnosing potential issues with keystrokes or mouse clicks, observing the effect of key mappings, or simply understanding how the X Window System and X server processes user inputs. 

## tldr 
 
> Print contents of X events.
> More information: <https://gitlab.freedesktop.org/xorg/app/xev>.

- Monitor all occurring X events:

`xev`

- Monitor all X events of the root window instead of creating a new one:

`xev -root`

- Monitor all X events of a particular window:

`xev -id {{window_id}}`

- Monitor X events from a given category (can be specified multiple times):

`xev -event {{event_category}}`
