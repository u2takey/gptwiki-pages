# terminalizer 
## chatgpt 
Terminalizer is a command-line tool that can be used to record and share your terminal sessions. The command "terminalizer" is used to start the tool and record your terminal session as a GIF or video. 

Here are the steps to use the terminalizer command:

1. Install terminalizer: You can install terminalizer using the npm package manager by running the following command in your terminal: 
```
npm install -g terminalizer
```

2. Start recording: To start recording your terminal session, you can run the following command:
```
terminalizer record mysession
```
This command will start recording your terminal session and save it to a file named "mysession.yml".

3. Customize your recording: You can customize your recording by creating a configuration file and applying it to your session. To create a configuration file, you can run the following command:
```
terminalizer config
```
This will create a configuration file named "terminalizer.yml" in your home directory.

You can then edit this file to customize your recording, such as changing the terminal font, background color, or recording settings.

To apply your configuration file to your session, you can run the following command:
```
terminalizer record mysession --config=/path/to/config.yml
```

4. Share your recording: Once you have recorded your terminal session, you can share it with others by exporting it as a GIF or video. To export as a GIF, you can run the following command:
```
terminalizer render mysession -o mysession.gif
```

To export as a video, you can run the following command:
```
terminalizer render mysession -o mysession.mp4 --quality high
```

This will export your terminal session as a high-quality video in the MP4 format. 

## tldr 
 
> Utility program which records the terminal and generate animated GIFs or share a video.
> More information: <https://terminalizer.com>.

- Create the global config directory:

`terminalizer init`

- Record the terminal and create a recording file:

`terminalizer record {{path/to/file}}`

- Play a recorded file on the terminal:

`terminalizer play {{path/to/file}}`

- Render a recording file as an animated GIF image:

`terminalizer render {{path/to/file}}`

- Upload a video to terminalizer.com:

`terminalizer share {{path/to/file}}`
