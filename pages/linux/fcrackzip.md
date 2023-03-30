# fcrackzip 
## chatgpt 
The "fcrackzip" command is a tool in Unix-based systems used for cracking password-protected zip files. Here is a breakdown of the command and its parameters:

Syntax: fcrackzip [options] file.zip

Options:
- b: Brute-force method
- c charset: Custom character list for brute-forcing
- D: Dictionary method
- l min-max: Password length range to check
- m crunch arg: Minimizing character set
- q: Quiet mode (reduce output)
- t threads: Number of threads to use
- u: Use unzip instead of built-in zip library
- V: Verbose mode (increase output)
- h: Help menu

Example: fcrackzip -b -c 'a,b,c' -l 6-8 myfile.zip

This command brute-forces a password for the "myfile.zip" archive. The charset option "-c" specifies a custom character list of lowercase "a", "b", and "c". The password length range "-l" is set to between 6 and 8 characters. The "-b" option specifies the brute-force method. If the password is discovered, it will be printed to the screen. 

## tldr 
 
> ZIP archive password cracking utility.
> More information: <https://manned.org/fcrackzip>.

- Brute-force a password with a length of 4 to 8 characters, and contains only alphanumeric characters (order matters):

`fcrackzip --brute-force --length 4-8 --charset aA1 {{archive}}`

- Brute-force a password in verbose mode with a length of 3 characters that only contains lowercase characters, `$` and `%`:

`fcrackzip -v --brute-force --length 3 --charset a:$% {{archive}}`

- Brute-force a password that contains only lowercase and special characters:

`fcrackzip --brute-force --length 4 --charset a! {{archive}}`

- Brute-force a password containing only digits, starting from the password `12345`:

`fcrackzip --brute-force --length 5 --charset 1 --init-password 12345 {{archive}}`

- Crack a password using a wordlist:

`fcrackzip --use-unzip --dictionary --init-password {{wordlist}} {{archive}}`

- Benchmark cracking performance:

`fcrackzip --benchmark`
