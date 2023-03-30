# isisdl 
## chatgpt 
Unfortunately, as an AI language model, I do not have access to the full context or environment in which the command "isisdl" is being used. Therefore, I cannot provide a detailed explanation of the command or its functions.

However, based on some research, "isisdl" is a command that is typically used in the context of NASA's Integrated Software for Imagers and Spectrometers (ISIS) software system, which is used for image processing and analysis of planetary science data. 

The "isisdl" command may refer to the "ISIS Data Loader," which is a tool for importing raw data files into the ISIS system. It may also refer to a specific executable or script within the ISIS software suite that performs a particular function related to data loading or management.

Without more context, it is difficult to provide a more detailed explanation of the "isisdl" command. 

## tldr 
 
> A downloading utility for ISIS of TU-Berlin. Download all your files and videos from ISIS.
> More information: <https://github.com/Emily3403/isisdl>.

- Start the synchronization process:

`isisdl`

- Limit the download rate to 20 MiB/s and download with 5 threads:

`isisdl --download-rate {{20}} --max-num-threads {{5}}`

- Run the initialization configuration wizard:

`isisdl --init`

- Run the additional configuration wizard:

`isisdl --config`

- Initiate a full synchronization of the database and compute the checksum of every file:

`isisdl --sync`

- Start ffmpeg to compress downloaded videos:

`isisdl --compress`
