# kosmorro 
## chatgpt 
As an AI language model, I am not sure about the specific command "kosmorro" as it does not have any recognized meanings, parameters, or functions in common programming languages or systems. 

However, I can suggest that it may be colloquial or domain-specific jargon in a specific community, game, or toolset that is not widely known. Nonetheless, without any additional context, it is tough to provide a detailed and accurate explanation. 

If you could provide more information about the context or system you encountered this command, I may be able to help you better. 

## tldr 
 
> Compute the ephemerides and the events for a given date, at a given position on Earth.
> More information: <http://kosmorro.space>.

- Get ephemerides for Paris, France:

`kosmorro --latitude={{48.7996}} --longitude={{2.3511}}`

- Get ephemerides for Paris, France, in the UTC+2 timezone:

`kosmorro --latitude={{48.7996}} --longitude={{2.3511}} --timezone={{2}}`

- Get ephemerides for Paris, France, on June 9th, 2020:

`kosmorro --latitude={{48.7996}} --longitude={{2.3511}} --date={{2020-06-09}}`

- Generate a PDF (note: TeXLive must be installed):

`kosmorro --format={{pdf}} --output={{path/to/file.pdf}}`
