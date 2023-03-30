# youtube-viewer 
## chatgpt 
youtube-viewer is a command-line tool that enables users to watch and search for videos directly from the terminal without opening any web browser. Here is a detailed explanation of the command:

The basic syntax of the command is as follows:

```
youtube-viewer [--help] [OPTIONS] [QUERY_STRING]
```

Where:

--help: Provides a quick overview of the command and its various options.

OPTIONS: The parameters or options that are used to customize the behavior of the youtube-viewer command. Some of the commonly used options include:

- --version: Displays the version information of the youtube-viewer command.

- --quality: Specifies the quality of the video playback.

- --format: Specifies the format of the video playback.

- --max-results: Specifies the maximum number of results to be displayed in the search results.

- --region: Specifies the region from which the videos should be searched.

- --color: Specifies the color scheme of the terminal.

QUERY_STRING: The search term or query string that is used to search for videos on YouTube. This can be a keyword, channel name, or URL.

Some of the important features of youtube-viewer command are:

- Supports various sorting and filtering options to refine the search results.

- Allows users to create and manage custom playlists.

- Provides a thumbnail preview of the videos before playing them.

- Supports keyboard shortcuts for easy navigation and control.

- Offers a wide range of customization options to adjust the playback quality, format, and other settings.

Overall, youtube-viewer is a handy tool for those who prefer to watch videos from the terminal or prefer a lightweight alternative to the YouTube website. 

## tldr 
 
> Command-line application for searching and playing videos from YouTube.
> More information: <https://github.com/trizen/youtube-viewer>.

- Search for a video:

`youtube-viewer {{search_term}}`

- Log in to your YouTube account:

`youtube-viewer --login`

- Watch a video with a specific URL in VLC:

`youtube-viewer --player={{vlc}} {{https://youtube.com/watch?v=dQw4w9WgXcQ}}`

- Display a search prompt and play the selected video in 720p:

`youtube-viewer -{{7}}`
