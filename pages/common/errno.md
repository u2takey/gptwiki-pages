# errno 
## chatgpt 
`errno` is not a command, but rather a variable in the C programming language. It is defined in the header file `<errno.h>` and allows the programmer to check for any error codes set by various system calls or library functions. 

When a function encounters an error condition, it typically sets an error code in `errno` that can be read and interpreted by the calling program. The value of `errno` is set to 0 (i.e., no error) at the beginning of the program or after a successful system call.

The program should always check `errno` after a system call or library function to determine if an error occurred. If `errno` is non-zero, the program should take appropriate action to handle the error, e.g., printing error messages, returning an error code, or exiting the program.

Here is an example of how to use `errno` in C programming:

```c
#include <stdio.h>
#include <errno.h>
#include <string.h>

int main() {
    FILE *file = fopen("nonexistentfile.txt", "r");
    if (file == NULL) {
        printf("Error opening file: %s\n", strerror(errno));
        return 1;
    }
    // do something with file
    fclose(file);
    return 0;
}
```

In this example, we attempt to open a file that does not exist. The `fopen` function will return NULL and set `errno` to a non-zero value indicating the error. We use the `strerror` function to convert the numeric value of `errno` to a human-readable error message and print it to the console. Finally, we return a non-zero value to indicate that there was an error in the program. 

## tldr 
 
> Look up errno names and descriptions.
> More information: <https://joeyh.name/code/moreutils/>.

- Lookup errno description by name or code:

`errno {{name|code}}`

- List all errno names, codes, and descriptions:

`errno --list`

- Search for code whose description contains all of the given text:

`errno --search {{text}}`

- Search for code whose description contains all of the given text (all locales):

`errno --search-all-locales {{text}}`
