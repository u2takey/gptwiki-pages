# import 
## chatgpt 
The "import" command is used in programming (specifically in Python) to bring in or access external code libraries, modules or packages which are required for a program to work properly or to add extra functionality to a program. 

When "importing" a library, the programmer is able to access functions, classes, variables or other resources that were previously defined within that library. 

For example, to use the "math" library in Python, the following import statement would be used:

```
import math
```

This statement makes all the functions and variables defined in the math library available for use in the current program. 

In addition, there are different ways to import libraries, such as:

- Importing only specific functions or variables from a library:

```
from math import sqrt
```

This statement only imports the "sqrt" function from the math library, making it available for use in the current program, but not other functions or variables in the library.

- Giving a library an alias:

```
import pandas as pd
```

This statement gives the Pandas library an alias "pd". Now, instead of typing out "pandas" every time you need to use it, you can simply use the "pd" alias. 

Overall, the "import" command is a fundamental tool that allows programmers to build more complex and powerful programs by utilizing pre-built libraries of code. 

## tldr 
 
> Capture some or all of an X server screen, and save the image to a file.
> Part of the ImageMagick library.
> More information: <https://imagemagick.org/script/import.php>.

- Capture the entire X server screen in the PostScript image format:

`import -window root {{output.postscript}}`

- Capture contents of a remote X server screen in the PNG format:

`import -window root -display {{remote_host}}:{{screen}}.{{display}} {{output.png}}`

- Capture a specific window, given its ID as displayed by `xwininfo`, into the JPEG format:

`import -window {{window_id}} {{output.jpg}}`
