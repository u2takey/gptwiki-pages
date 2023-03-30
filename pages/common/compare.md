# compare 
## chatgpt 
The "compare" command is used to compare two files and identify the differences between them. It is commonly used to check whether two versions of a file are identical or not. 

The basic syntax of the compare command is:

compare [options] file1 file2

Where "options" can be different parameters that modify the behavior of the command, and "file1" and "file2" are the names of the files to be compared.

Some common options of the compare command are:

- "-l": displays differences as the characters that differ with their respective ASCII code.
- "-i": ignores the differences in case.
- "-w": ignores whitespace and blank lines.
- "-B": ignores changes in the amount of white space between words.

After executing the command, if there are differences between the two files, the command will display them on the screen. The differences are usually colored to make them easily visible. If the files are identical, the command will display no output.

Overall, the compare command is a useful tool for identifying differences between files and ensuring that files have not been tampered with or corrupted. 

## tldr 
 
> View the difference between 2 images.
> More information: <https://imagemagick.org/script/compare.php>.

- Compare 2 images:

`compare {{image1.png}} {{image2.png}} {{diff.png}}`

- Compare 2 images using a custom metric:

`compare -verbose -metric {{PSNR}} {{image1.png}} {{image2.png}} {{diff.png}}`
