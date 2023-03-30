# wodim 
## chatgpt 
The `wodim` command is a tool for burning CDs, DVDs, and Blu-rays on Unix-like systems. It is a command-line utility that supports a wide range of commands and options. Here are some of the key features and functions of the `wodim` command:

1. Burning ISO images: `wodim` can burn ISO images to a CD, DVD, or Blu-ray disc. This is done by specifying the path to the ISO image file as an argument to the `wodim` command.

Example: `wodim -v -dao dev=/dev/cdrom image.iso`

2. Erasing Discs: `wodim` can erase a rewritable disc before burning a new image. This is done by specifying the `blank=fast` or `blank=all` option depending on whether you want to quickly erase the disc or completely erase it.

Example: `wodim blank=fast dev=/dev/cdrom`

3. Creating Audio CDs:  `wodim` can create an audio CD by specifying the source audio files as an argument to the `wodim` command.

Example: `wodim -v -dao dev=/dev/cdrom audio1.wav audio2.wav`

4. Verifying Discs: `wodim` can be used to verify the data on a burned disc. This is done by specifying the `fs=iso` option which checks the integrity of the file system on the disc.

Example: `wodim -v -toc -fs=iso dev=/dev/cdrom`

5. Writing to Multiple Writers: `wodim` can write data to multiple writers at the same time by specifying the device paths of the additional writers as arguments.

Example: `wodim dev=/dev/cdrom dev=/dev/cdrom2 image.iso`

These are some of the key features and functions of the `wodim` command that can be used for burning and managing discs on Unix-like systems. 

## tldr 
 
> Command (aliased as `cdrecord` on some systems) for recording data to CDs or DVDs.
> Some invocations of wodim can cause destructive actions, such as erasing all the data on a disc.
> More information: <https://manned.org/wodim>.

- Display optical drives available to `wodim`:

`wodim --devices`

- Record ("burn") an audio-only disc:

`wodim dev=/dev/{{optical_drive}} -audio {{track*.cdaudio}}`

- Burn a file to a disc, ejecting the disc once done (some recorders require this):

`wodim -eject dev=/dev/{{optical_drive}} -data {{file.iso}}`

- Burn a file to the disc in an optical drive, potentially writing to multiple discs in succession:

`wodim -tao dev=/dev/{{optical_drive}} -data {{file.iso}}`
