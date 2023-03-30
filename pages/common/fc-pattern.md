# fc-pattern 
## chatgpt 
The command "fc-pattern" is a Linux command used to display the fontconfig pattern matching system. It is used for customizing the fonts used by different applications on a Linux system. 

The "fc-pattern" command works by querying the fontconfig system and displaying the available fonts, their properties, and how they can be used by applications. It returns information such as the font family, font style (bold, italic, etc.), font weight, and other attributes that can be used to customize a font.

Using the "fc-pattern" command, users can view and modify fontconfig patterns to customize the fonts used by specific applications or system-wide. For example, if a user wants to set a specific font for a particular application, they can use the "fc-pattern" command to find the appropriate font and modify its properties as required.

Overall, "fc-pattern" is a useful command for Linux users who want to customize their font settings and ensure that their system displays fonts in a consistent and pleasing way. 

## tldr 
 
> Shows information about a font matching a pattern.
> More information: <https://manned.org/fc-pattern>.

- Display default information about a font:

`fc-pattern --default '{{DejaVu Serif}}'`

- Display config information about a font:

`fc-pattern --config '{{DejaVu Serif}}'`
