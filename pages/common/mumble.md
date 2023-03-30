# mumble 
## chatgpt 
As an AI language model, I can explain the mumble command and its basic functions, but I may not have the ability to use it practically as it may require specific software or hardware configurations. 

Mumble is a free and open-source, low-latency, high-quality voice chat software that allows users to communicate with each other in real time. The mumble command is used to start the Mumble client application from the command line interface (CLI).

When you run the mumble command, Mumble launches a graphical user interface (GUI) where you can connect to your preferred Mumble server or create your own server. You can join existing chat rooms or create your own chat room, and have private conversations with individual users or groups.

Here's a quick rundown of some of the basic command options you can use with the mumble command:

-m / --minimal: Starts Mumble in minimal mode, which disables most of its UI features in favor of a simpler interface.

-c / --config: Specifies the path to the Mumble configuration file. By default, Mumble looks for the configuration file in the user's home directory.

-s / --server: Specifies the Mumble server to connect to by providing its IP address or hostname.

-p / --password: Allows you to specify the password to authenticate with the Mumble server.

There are many more advanced options available for the Mumble client, but these are some of the most commonly used options associated with the mumble command. 

## tldr 
 
> Low-latency, high quality voice chat software.
> More information: <https://www.mumble.info>.

- Open Mumble:

`mumble`

- Open Mumble and immediately connect to a server:

`mumble mumble://{{username}}@{{example.com}}`

- Open Mumble and immediately connect to a password protected server:

`mumble mumble://{{username}}:{{password}}@{{example.com}}`

- Mute/unmute the microphone in a running Mumble instance:

`mumble rpc {{mute|unmute}}`

- Mute/unmute the microphone and the audio output of Mumble:

`mumble rpc {{deaf|undeaf}}`
