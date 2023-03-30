# units 
## chatgpt 
The "units" command is a built-in utility in Unix/Linux operating systems that converts quantities between different measurements of physical units such as length, volume, speed, temperature, etc. 

When the "units" command is executed in a terminal, it opens an interactive mode, where the user can enter the units they want to convert from and to. The syntax for using the "units" command is:

units [input_units] [output_units]

For example, to convert 12 inches to centimeters, you can type:

```
units inch cm
```

Then, you can enter the quantity you want to convert, in this case, 12:

```
12
```

The "units" command will then output the converted value:

```
30.48
```

Another way to use the "units" command is to pipe input/output units and values directly into it as arguments. For example, to convert 5 miles per hour to kilometers per hour, you can type:

```
echo "5 mi/h" | units -t "km/h"
```

The "-t" option tells "units" to output a terse output, without any explanation, and the quoted strings define the input/output units. The command will output:

```
8.04672
```

which is the converted value in kilometers per hour.

Overall, the "units" command is a convenient and powerful tool for converting between different units of measurement in Unix/Linux environments, and it supports a wide range of units and dimensions. 

## tldr 
 
> Provide the conversion between two units of measure.
> More information: <https://www.gnu.org/software/units/>.

- Run in interactive mode:

`units`

- List all units containing a specific string in interactive mode:

`search {{string}}`

- Show the conversion between two simple units:

`units {{quarts}} {{tablespoons}}`

- Convert between units with quantities:

`units "{{15 pounds}}" {{kilograms}}`

- Show the conversion between two compound units:

`units "{{meters / second}}" "{{inches / hour}}"`

- Show the conversion between units with different dimensions:

`units "{{acres}}" "{{ft^2}}"`

- Show the conversion of byte multipliers:

`units "{{15 megabytes}}" {{bytes}}`
