# boot 
## chatgpt 
The command "boot" is a command used in computer systems to initiate the system booting process. The process is responsible for loading the operating system and its related files into the memory and launching it so that the computer is ready to use.

When the command is executed, the computer's firmware (BIOS, UEFI) starts running the power-on self-test (POST) process, which checks the system hardware and ensures that it is working correctly. The firmware then looks for the boot sector on the computer's storage devices like hard drives, SSDs, USB flash drives, DVDs or network boot server, and loads the boot loader into the memory.

The boot loader is a small program that is responsible for loading the kernel and any necessary drivers and modules needed to run the operating system. Once the boot loader has finished loading the necessary files, the operating system starts initializing and the computer boots up.

The "boot" command can be initiated in different ways depending on the system used such as pressing the power button, selecting "restart" or "boot" from the operating system, or by selecting a boot device from the firmware settings.

Overall, the "boot" command is an essential command in computing systems as it is responsible for initiating and launching the operating system to ensure that the computer is ready to use. 

## tldr 
 
> Build tooling for the Clojure programming language.
> More information: <https://github.com/boot-clj/boot>.

- Start a REPL session either with the project or standalone:

`boot repl`

- Build a single `uberjar`:

`boot jar`

- Learn about a command:

`boot cljs --help`

- Generate scaffolding for a new project based on a template:

`boot --dependencies boot/new new --template {{template_name}} --name {{project_name}}`

- Build for development (if using the boot/new template):

`boot dev`

- Build for production (if using the boot/new template):

`boot prod`
