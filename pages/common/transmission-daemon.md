# transmission-daemon 
## chatgpt 
Transmission-daemon is a command used in Linux-based systems to start the Transmission BitTorrent client as a server. This means that Transmission will be running as a background process, constantly monitoring and downloading the torrents specified in its queue.

The daemon version of Transmission is useful for users who want to use the client headlessly or remotely, via a web interface or a remote client. It's also useful for users who want to conserve system resources, as the daemon version takes up less memory and CPU usage than the GUI version.

The command to start transmission-daemon is simply "transmission-daemon". When executed, the daemon starts running in the background, and can be controlled via a web interface (by default at http://localhost:9091/transmission/web/) or a remote client that supports the Transmission RPC protocol.

Some common options that can be passed to the transmission-daemon command include:

- -g [config dir]: Specifies a different configuration directory for Transmission. By default, it uses ~/.config/transmission-daemon/.
- -f: Runs Transmission in the foreground instead of as a background process.
- -p [port]: Specifies a different port for the web interface. By default, it uses port 9091.
- -w [watch dir]: Specifies a different watch directory for new torrents. By default, it uses ~/.config/transmission-daemon/watch/.

Overall, the transmission-daemon command is a simple and powerful way to run a BitTorrent client on a Linux-based system. It can be customized with various options and used remotely, making it a versatile tool for downloading and managing torrents. 

## tldr 
 
> Daemon controlled with `transmission-remote` or its web interface.
> See also: `transmission`.
> More information: <https://manned.org/transmission-daemon>.

- Start a headless `transmission` session:

`transmission-daemon`

- Start and watch a specific directory for new torrents:

`transmission-daemon --watch-dir {{path/to/directory}}`

- Dump daemon settings in JSON format:

`transmission-daemon --dump-settings > {{path/to/file.json}}`

- Start with specific settings for the web interface:

`transmission-daemon --auth --username {{username}} --password {{password}} --port {{9091}} --allowed {{127.0.0.1}}`
