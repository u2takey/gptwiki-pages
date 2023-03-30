# calendar 
## chatgpt 
The command `calendar` is a simple utility in Unix-like operating systems that displays a calendar for a given month or year (or the current month if no arguments are provided). The `calendar` command is used in the terminal to display the calendar of the current month and year.

Syntax:

```shell
calendar [month] [year]
```

If the `month` and `year` arguments are not given, the calendar for the current month and year will be displayed. If only the `month` argument is given, the calendar for that month and the current year will be displayed. If both `month` and `year` arguments are given, the calendar for that month and year will be displayed.

A typical output of the `calendar` command will look like:

```
     October 2021      
Su Mo Tu We Th Fr Sa  
                1  2  
 3  4  5  6  7  8  9  
10 11 12 13 14 15 16  
17 18 19 20 21 22 23  
24 25 26 27 28 29 30  
31 
```

In the output of the above example, the current month and year name are displayed at the top of the calendar, and the days of the month are displayed in a grid format with the days of the week as column headers.

Overall, the `calendar` command is a useful tool for quickly checking the calendar of a given month or year, especially for scheduling events or appointments. 

## tldr 
 
> Display upcoming events from a calendar file.
> More information: <https://www.commandlinux.com/man-page/man1/calendar.1.html>.

- Show events for today and tomorrow (or the weekend on Friday) from the default calendar:

`calendar`

- Look [A]head, showing events for the next 30 days:

`calendar -A {{30}}`

- Look [B]ack, showing events for the previous 7 days:

`calendar -B {{7}}`

- Show events from a custom calendar [f]ile:

`calendar -f {{path/to/file}}`
