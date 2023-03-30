# packer 
## chatgpt 
Packer is a command-line tool used for creating machine images (such as virtual machines or containers) for various platforms, such as Amazon Web Services or Microsoft Azure. The tool works by defining a set of machine configurations using a configuration file, which can be in JSON format. The configurations specify things like the operating system, any software to be installed, and configuration settings.

When the Packer command is run, it reads the configuration file and creates a new machine image based on the specified configuration. This image can then be used to create new instances of the machine type on the target platform.

Some common options that can be used with the Packer command include:

- validate: checks the syntax of the Packer configuration file
- build: creates a new machine image based on the Packer configuration file
- inspect: displays information about the Packer template, including all build actions and provisioning steps
- version: displays the version of Packer that is currently being used. 

Overall, Packer simplifies the process of creating machine images, making it easier to manage and deploy infrastructure across multiple platforms. 

## tldr 
 
> Build automated machine images.
> More information: <https://www.packer.io/>.

- Build an image:

`packer build {{path/to/config.json}}`

- Check the syntax of a Packer image config:

`packer validate {{path/to/config.json}}`
