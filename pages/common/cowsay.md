# cowsay 
## chatgpt 
cowsay is a command line utility available on Unix-based systems, it is used to generate ASCII art of a cow and display a message given as an argument. This command is often used for amusement, non-serious communication and demonstration purposes.

When you run the cowsay command, it will by default display the ASCII art of a cow, and will prompt you to enter a message. Once you enter a message and hit enter, the cow will speak the message you entered, which will be displayed underneath the ASCII art.

For example, if you run the command “cowsay Hello there!” the output will be as follows:

 ___________
< Hello there! >
 -----------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                 ||----w |
                 ||     ||

As you can see, the message "Hello there!" is displayed on the next line, and it appears that the cow is saying it. 

The cowsay command has various options, some of which include changing the character used to generate the ASCII art, changing the speech bubbles, and modifying the message alignment. 

## tldr 
 
> Print ASCII art (by default a cow) saying or thinking something.
> More information: <https://github.com/tnalpgge/rank-amateur-cowsay>.

- Print an ASCII cow saying "hello, world":

`cowsay "{{hello, world}}"`

- Print an ASCII cow saying text from `stdin`:

`echo "{{hello, world}}" | cowsay`

- List all available art types:

`cowsay -l`

- Print the specified ASCII art saying "hello, world":

`cowsay -f {{art}} "{{hello, world}}"`

- Print a dead thinking ASCII cow:

`cowthink -d "{{I'm just a cow, not a great thinker...}}"`

- Print an ASCII cow with custom eyes saying "hello, world":

`cowsay -e {{characters}} "{{hello, world}}"`
