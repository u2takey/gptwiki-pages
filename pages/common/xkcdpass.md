# xkcdpass 
## chatgpt 
xkcdpass is a command used to generate a random password composed of a sequence of random words. This tool generates passwords that are more secure than traditional passwords as they are more difficult to crack by password-guessing software. xkcdpass is based on the concept introduced by Randall Munroe, the creator of the webcomic XKCD, which states that a password composed of random words is easier to remember and harder to crack than a traditional password that includes numbers, letters, and symbols.

When executed, xkcdpass generates a sequence of four or more random words that can be used as a password. The length of the password, the number of words it contains, and other options can be specified by the user.

xkcdpass uses a dictionary file containing thousands of words to generate the password. The tool selects the words at random and combines them into a passphrase. The dictionary can be customized or replaced with one of your own choosing.

Overall, xkcdpass is a simple yet effective way to generate strong, memorable passwords that can help keep your sensitive information secure. 

## tldr 
 
> A flexible and scriptable password generator which generates strong passphrases.
> Inspired by XKCD 936.
> More information: <https://github.com/redacted/XKCD-password-generator>.

- Generate one passphrase with the default options:

`xkcdpass`

- Generate one passphrase whose first letters of each word match the provided argument:

`xkcdpass -a {{acrostic}}`

- Generate passwords interactively:

`xkcdpass -i`
