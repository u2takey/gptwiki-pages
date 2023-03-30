# hashid 
## chatgpt 
hashid is a command-line tool designed to identify the different types of hash codes that are commonly used in computing systems. When you run the hashid command, it analyzes a string of characters, identifies the hash algorithm used to create that string, and displays information about it.

The information displayed by hashid may include the algorithm used, the length of the hash, the name of the hash, and an estimate of how long it would take to crack the hash. In addition to generating this information, hashid can also analyze files and directories containing hashes, and it can be used to compare two different hashes and determine if they are the same.

Here are some examples of how to use the hashid command:

- To identify the type of hash for a specific string of characters, simply type the string after the command:

  hashid "admin123"
  
- To analyze a file containing many different types of hashes, use the -f (file) option and specify the path to the file:

  hashid -f /path/to/hashes.txt
  
- To compare two different hashes, use the -m (mode) option followed by the hashes:

  hashid -m "74b87337454200d4d33f80c4663dc5e5" "f3ada405ce890b6f8204094deb12d8a8"

Overall, hashid is a useful tool for anyone working with hashes and needing to determine the algorithm used to create them. 

## tldr 
 
> Python3 program that identifies data and password hashes.
> More information: <https://github.com/psypanda/hashID>.

- Identify hashes from standard input (through typing, copying and pasting, or piping the hash into the program):

`hashid`

- Identify hashes passed as arguments (multiple hashes can be passed):

`hashid {{hash}}`

- Identify hashes on a file (one hash per line):

`hashid {{path/to/hashes.txt}}`

- Show all possible hash types (including salted hashes):

`hashid --extended {{hash}}`

- Show `hashcat`'s mode number and `john`'s format string of the hash types:

`hashid --mode --john {{hash}}`

- Save output to a file instead of printing to standard output:

`hashid --outfile {{path/to/output.txt}} {{hash}}`
