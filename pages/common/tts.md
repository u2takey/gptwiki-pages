# tts 
## chatgpt 
The command "tts" stands for "text-to-speech". It is a computer program that converts written text into spoken words. 

In the context of programming or scripting, the use of the "tts" command is to allow computers or devices to read texts out loud. This can be done through various programming languages, libraries, or APIs.

The tts command can be used for various purposes such as accessibility, language learning, audiobook creation, or automated voice response systems. It typically requires a text input (such as a string variable or a file) and a voice engine, which is responsible for generating the speech from the text. The output of the tts command can be played back through speakers or saved as an audio file.

Overall, the tts command provides a way for written language to be translated into speech, allowing for greater accessibility and convenience in various applications. 

## tldr 
 
> Synthesize speech on the command line.
> More information: <https://github.com/coqui-ai/TTS#command-line-tts>.

- Run text-to-speech with the default models, writing the output to "tts_output.wav":

`tts --text "{{text}}"`

- List provided models:

`tts --list_models`

- Query info for a model by idx:

`tts --model_info_by_idx {{model_type/model_query_idx}}`

- Query info for a model by name:

`tts --model_info_by_name {{model_type/language/dataset/model_name}}`

- Run a text-to-speech model with its default vocoder model:

`tts --text "{{text}}" --model_name {{model_type/language/dataset/model_name}}`

- Run your own text-to-speech model (using the Griffin-Lim vocoder):

`tts --text "{{text}}" --model_path {{path/to/model.pth}} --config_path {{path/to/config.json}} --out_path {{path/to/file.wav}}`
