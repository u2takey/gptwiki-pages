# reflector 
## chatgpt 
The "reflector" command is a utility in the Arch Linux operating system which is used to perform a variety of tasks related to maintaining and optimizing the system's package mirrors. 

When you run this command, it will contact a server to check the most up-to-date package mirror list, and then use this information to generate a new mirrorlist file. This new file is a list of the fastest and most reliable mirrors for downloading packages, and is used by the system to ensure that package updates and installations are as fast and efficient as possible. 

The "reflector" command can be used to perform a range of tasks, including specifying a custom mirror URL or location, setting bandwidth limits for the mirror synchronization process, and filtering mirrors by country or other criteria. It can also be used to test the download speed of different mirrors, so you can choose the fastest one for your system. 

Overall, the "reflector" command is a useful tool for managing and optimizing the package mirrors used by your Arch Linux system. By keeping your mirrorlist up-to-date and choosing the fastest and most reliable mirrors, you can ensure that your system updates and installations are as smooth and efficient as possible. 

## tldr 
 
> Arch script to fetch and sort mirrorlists.
> More information: <https://manned.org/reflector>.

- Get all mirrors, sort for download speed and save them:

`sudo reflector --sort {{rate}} --save {{/etc/pacman.d/mirrorlist}}`

- Only get German HTTPS mirrors:

`reflector --country {{Germany}} --protocol {{https}}`

- Only get the 10 recently sync'd mirrors:

`reflector --latest {{10}}`
