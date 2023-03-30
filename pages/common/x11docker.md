# x11docker 
## chatgpt 
x11docker is a command-line tool used to run Linux GUI applications and desktop environments in Docker containers while preserving the host system's look and feel. It works by creating a secure isolated environment for each application and then connecting it with the underlying X server display.

The x11docker command has several options and arguments that allow users to specify the name of the Docker image to use, mount volumes, assign CPU and memory resources, and set environment variables. For instance, the basic syntax for running an application with x11docker would look like this:

```
$ x11docker some/image firefox
```

This will launch Firefox inside a Docker container with the "some/image" Docker image.

Other commonly used options with x11docker include:

- `-d` to run the container in detached mode (i.e., without attaching to its console output)
- `-e` to pass environment variables to the container
- `--gpu` to enable GPU acceleration for specific applications
- `-v` to mount volumes inside the container

Using x11docker can be especially useful in situations where isolation or compatibility are concerns. For example, developers may want to test code in different Linux environments or users may need to run legacy applications that cannot run in the latest version of their operating system. 

## tldr 
 
> Securely run GUI applications and desktop UIs in Docker containers.
> See also `xephyr`.
> More information: <https://github.com/mviereck/x11docker>.

- Launch VLC in a container:

`x11docker --pulseaudio --share={{$HOME/Videos}} {{jess/vlc}}`

- Launch Xfce in a window:

`x11docker --desktop {{x11docker/xfce}}`

- Launch GNOME in a window:

`x11docker --desktop --gpu --init={{systemd}} {{x11docker/gnome}}`

- Launch KDE Plasma in a window:

`x11docker --desktop --gpu --init={{systemd}} {{x11docker/kde-plasma}}`

- Display help:

`x11docker --help`
