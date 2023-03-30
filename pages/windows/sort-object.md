# Sort-Object 
## chatgpt 
Sort-Object is a PowerShell cmdlet that sorts objects in a collection based on specified properties. 

The syntax for the Sort-Object cmdlet is as follows: 

Sort-Object [-Property] <String[]> [-Ascending] [-Descending] [-CultureInvariant] [-Unique] [<CommonParameters>]

Let's break down each parameter:

- Property: This parameter specifies the object property that should be used to sort the objects. You can specify one or more properties as an array of strings.

- Ascending: This parameter sorts the objects in ascending order (smallest to largest) based on the values of the specified property. If not set, the default is ascending order.

- Descending: This parameter sorts the objects in descending order (largest to smallest) based on the values of the specified property.

- CultureInvariant: This parameter sorts the objects in a culture-invariant manner. This ignores cultural differences in language and formatting and sorts based solely on the values of the specified property.

- Unique: This parameter removes duplicates from the collection before sorting the objects.

- CommonParameters: These are parameters that are available to all PowerShell cmdlets.

In summary, the Sort-Object cmdlet is used to sort objects in a collection based on specified properties. It offers several parameters to customize the sorting behavior. 

## tldr 
 
> Sorts objects by property values.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/sort-object>.

- Sort the current directory by name:

`Get-ChildItem | Sort-Object`

- Sort the current directory by name descending:

`Get-ChildItem | Sort-Object -Descending`

- Sort items removing duplicates:

`"a", "b", "a" | Sort-Object -Unique`

- Sort the current directory by file length:

`Get-ChildItem | Sort-Object -Property Length`

- Sort processes with the highest memory usage based on their working set (WS) size:

`Get-Process | Sort-Object -Property WS`
