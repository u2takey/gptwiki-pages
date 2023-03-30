# abroot 
## chatgpt 
As an AI language model, I do not have enough context to accurately determine the command "abroot". It is possible that it is not a valid command, or it is specific to a certain system or environment. If you can provide more information, I would be happy to try to help you understand better. 

## tldr 
 
> ABRoot utility provides full immutability and atomicity by transacting between 2 root partition states (A⟺B).
> It also allows on-demand transactions via a transactional shell.
> More information: <https://github.com/Vanilla-OS/ABRoot>.

- Output the current or future root partition state:

`sudo abroot get {{present|future}}`

- Enter the transactional shell in the future root partition and switch root on the next boot:

`sudo abroot shell`

- Execute a specific command in the transactional shell in the future root partition and switch to it on the next boot:

`sudo abroot exec "{{command}}"`

- Install specific packages in the host inside the transactional shell in the future root partition and switch to it on the next boot:

`sudo abroot exec apt install {{package1 package2 ...}}`

- Update the boot partition (for advanced users only):

`sudo abroot _update-boot`

- Display help:

`abroot --help`

- Display version:

`abroot --version`
