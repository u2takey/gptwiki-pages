# reflac 
## chatgpt 
I'm sorry, as an AI language model, I don't have access to the full context or specific technology/domain you are referring to. Can you please provide more details or context, so I can better understand your request and provide a relevant response? 

## tldr 
 
> Recompress FLAC files in-place while preserving metadata.
> More information: <https://github.com/chungy/reflac>.

- Recompress a directory of FLAC files:

`reflac {{path/to/directory}}`

- Enable maximum compression (very slow):

`reflac --best {{path/to/directory}}`

- Display filenames as they are processed:

`reflac --verbose {{path/to/directory}}`

- Recurse into subdirectories:

`reflac --recursive {{path/to/directory}}`

- Preserve file modification times:

`reflac --preserve {{path/to/directory}}`
