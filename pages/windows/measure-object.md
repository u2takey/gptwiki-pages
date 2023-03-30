# Measure-Object 
## chatgpt 
The Measure-Object command is a PowerShell cmdlet that is used to calculate the numerical properties of an object, such as the count, average, sum, minimum, and maximum. It is commonly used to measure the size and complexity of data sets or to provide aggregate statistics about data.

Here's an overview of the Measure-Object command and how it works:

- The Measure-Object command calculates numerical properties of the input that is piped or passed to it. For example, you could pipe a list of numbers, words, or any other object to the Measure-Object command and it will calculate different types of properties.
- By default, the Measure-Object command returns the total count of the input object. However, you can use various parameters to specify different types of calculations, such as Average, Sum, Minimum, Maximum, and more.
- The Measure-Object command can be used to measure the size and complexity of data sets, such as the number of files in a directory, the size of a file, or the number of rows and columns in a data table.
- The Measure-Object command is often used in PowerShell scripts to provide aggregate statistics about data, such as the average length of a string, the total size of a directory, or the number of occurrences of a certain word in a text file.

Overall, the Measure-Object command is a powerful and flexible tool for calculating numerical properties of an object in PowerShell, and it can help automate many data analysis tasks. 

## tldr 
 
> Calculates the numeric properties of objects, and the characters, words, and lines in string objects, such as files of text.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/measure-object>.

- Count the files and folders in a directory:

`Get-ChildItem | Measure-Object`

- Pipe input to Measure-Command (objects that are piped to `Measure-Command` are available to the script block that is passed to the Expression parameter):

`"One", "Two", "Three", "Four" | Set-Content -Path "{{path\to\file}}"; Get-Content "{{path\to\file}}"; | Measure-Object -Character -Line -Word`
