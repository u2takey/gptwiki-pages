# kdocker 
## chatgpt 
Kdocker is a command line utility in Linux that allows users to minimize or dock any application/window into the system tray or the panel.

The basic command syntax for kdocker is:

kdocker [options] command

Here, 'command' represents the application, window or process you want to dock.

Some of the commonly used options with kdocker are:

- --icon - specifies the icon to be displayed in the system tray or panel
- --name - sets the name of the docked application
- --transparency - specifies the level of transparency for the docked application/window
- --hidden - hides the application/window when it is docked
- --ontop - keeps the application/window on top even when it is minimized
- --ontop-click - allows users to click on the docked application/window even when it is on top

To use kdocker, first install it through the package manager of your Linux distribution. After installing, open a terminal window and type the kdocker command followed by the name of the application you want to dock. For example, to dock the Firefox browser, you can run the following command:

kdocker --icon firefox firefox

This will minimize the Firefox window to the system tray or panel. To restore it, simply click on the kdocker icon in the system tray/panel.

Overall, kdocker is a useful utility for managing application windows and keeping your workspace clutter-free by minimizing them to the system tray or panel. 

## tldr 
 
> Easily dock applications to the system tray.
> More information: <https://github.com/user-none/KDocker>.

- Display a cursor to send a window to the system tray when pressing the left mouse button (press any other mouse button to cancel):

`kdocker`

- Open an application and send it to the system tray:

`kdocker {{application}}`

- Send focused window to the system tray:

`kdocker -f`

- Display a cursor to send a window to the system tray with a custom icon when pressing the left mouse button:

`kdocker -i {{/path/to/icon}}`

- Open an application, send it to the system tray and if focus is lost, minimize it:

`kdocker -l {{application}}`

- Print version:

`kdocker --version`
