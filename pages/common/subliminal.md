# subliminal 
## chatgpt 
The `subliminal` command is a Python tool used for downloading and synchronizing subtitles for movies and TV shows. It can be used to search for subtitles in multiple languages from websites such as OpenSubtitles, Podnapisi, and Subscene. The command has several subcommands that allow you to perform different tasks:
- `download`: This subcommand downloads subtitles in the specified language for a given video file. You will need to provide the path to the video file and specify the language for the subtitles.
- `list`: This subcommand lists the available subtitles for a given video file. You will need to provide the path to the video file and specify the language for the subtitles.
- `cache`: This subcommand lists, removes, or changes the cache directory used by the tool.
- `clean`: This subcommand cleans up the cache and all downloaded subtitle files.
- `config`: This subcommand allows you to view and edit the configuration file for the tool.
- `providers`: This subcommand lists the available providers that can be used to search for subtitles.
- `rehash`: This subcommand recalculates the hash of a given video file and updates the associated subtitle files.

Overall, the `subliminal` command is a powerful tool for ensuring you have subtitles for your favorite movies and TV shows. 

## tldr 
 
> Python-based subtitle downloader.
> More information: <https://github.com/Diaoul/subliminal>.

- Download English subtitles for a video:

`subliminal download -l {{en}} {{video.ext}}`
