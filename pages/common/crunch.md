# crunch 
## chatgpt 
The "crunch" command is a tool used for creating custom wordlists, passwords and character sets for various security testing purposes. 

The command has a number of options that can be used to generate the desired output. Some of the commonly used options are:

1. -t: This option allows you to specify a template which decides the structure of the output. For example, you could create a custom dictionary that follows the structure of email addresses, phone numbers or usernames. 

2. -c: This option lets you specify the character set for generating words. You can specify a range of characters like upper-case, lower-case, numbers, symbols, etc. 

3. -o: This option allows you to specify a file where the output will be saved. If this option is not used, the output will be printed to the terminal. 

4. -b: This option lets you specify the minimum and maximum length of the generated words. 

5. -s: This option lets you skip a specific number of characters before generating the output. 

Overall, the "crunch" command is a powerful utility tool for generating custom wordlists and character sets which can be used for a wide range of cybersecurity applications. 

## tldr 
 
> Wordlist generator.
> More information: <https://sourceforge.net/projects/crunch-wordlist/>.

- Output a list of words of length 1 to 3 with only lowercase characters:

`crunch {{1}} {{3}}`

- Output a list of hexadecimal words of length 8:

`crunch {{8}} {{8}} {{0123456789abcdef}}`

- Output a list of all permutations of abc (lengths are not processed):

`crunch {{1}} {{1}} -p {{abc}}`

- Output a list of all permutations of the given strings (lengths are not processed):

`crunch {{1}} {{1}} -p {{abc}} {{def}} {{ghi}}`

- Output a list of words generated according to the given pattern and a maximum number of duplicate letters:

`crunch {{5}} {{5}} {{abcde123}} -t {{@@@12}} -d 2@`

- Write a list of words in chunk files of a given size, starting with the given string:

`crunch {{3}} {{5}} -o {{START}} -b {{10kb}} -s {{abc}}`

- Write a list of words stopping with the given string and inverting the wordlist:

`crunch {{1}} {{5}} -o {{START}} -e {{abcde}} -i`

- Write a list of words in compressed chunk files with a specified number of words:

`crunch {{1}} {{5}} -o {{START}} -c {{1000}} -z {{gzip|bzip2|lzma|7z}}`
