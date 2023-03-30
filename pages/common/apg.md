# apg 
## chatgpt 
`apg` is a command-line tool that generates random passwords. The name `apg` stands for Automated Password Generator. When you run the `apg` command, it will output a randomly generated password.

The `apg` command has various options that you can use to customize the generated password. Some of the most commonly used options are:

- `-a` or `--no-capitalize`: This option will prevent the generator from using capital letters in the password.
- `-c` or `--capitalize`: This option will force the generator to use at least one capital letter in the password.
- `-n [num]` or `--num-passwords=[num]`: This option will generate multiple passwords at once. You can specify the number of passwords you want to generate by replacing `[num]` with the desired number.
- `-M [num]` or `--min-length=[num]`: This option will set the minimum length of the password to `[num]`.
- `-x [num]` or `--max-length=[num]`: This option will set the maximum length of the password to `[num]`.

For example, if you want to generate a password with a minimum length of 12 characters and no capital letters, you can run the command `apg -a -M 12`. If you want to generate 5 passwords at once, you can run the command `apg -n 5`. 

## tldr 
 
> Creates arbitrarily complex random passwords.
> More information: <https://manned.org/apg>.

- Create random passwords (default password length is 8):

`apg`

- Create a password with at least 1 symbol (S), 1 number (N), 1 uppercase (C), 1 lowercase (L):

`apg -M SNCL`

- Create a password with 16 characters:

`apg -m {{16}}`

- Create a password with maximum length of 16:

`apg -x {{16}}`

- Create a password that doesn't appear in a dictionary (the dictionary file has to be provided):

`apg -r {{dictionary_file}}`
