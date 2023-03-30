# ncal 
## chatgpt 
The command "ncal" is used to display the calendar of the current or specified month. It stands for "new calendar".

The basic syntax of the command is:

ncal [options] [month] [year]

If no arguments are given, it displays the calendar of the current month.

Options:

- -m : displays the calendar of the specified month.
- -y : displays the calendar of the specified year.
- -w : displays the calendar in wide format.
- -h : displays the calendar in a horizontal format.
- -e : highlights the current date with an asterisk.
- -b : displays output in black and white.
- -C : shows the specified year in a two-digit or four-digit format.

Examples:

1. To display the current month's calendar:

$ ncal

Output:

   September 2021
Mo Tu We Th Fr Sa Su
       1  2  3  4  5
 6  7  8  9 10 11 12
13 14 15 16 17 18 19
20 21 22 23 24 25 26
27 28 29 30      

2. To display the calendar of a specific month:

$ ncal -m 11

Output:

    November 2021
Mo Tu We Th Fr Sa Su
 1  2  3  4  5  6  7
 8  9 10 11 12 13 14
15 16 17 18 19 20 21
22 23 24 25 26 27 28
29 30              

3. To display the calendar of a specific year:

$ ncal -y 2022

Output:

                                2022
      January                  February                  March
Mo Tu We Th Fr Sa Su    Mo Tu We Th Fr Sa Su    Mo Tu We Th Fr Sa Su
                1  2          1  2  3  4  5  6          1  2  3  4  5
 3  4  5  6  7  8  9     7  8  9 10 11 12 13     6  7  8  9 10 11 12
10 11 12 13 14 15 16    14 15 16 17 18 19 20    13 14 15 16 17 18 19
17 18 19 20 21 22 23    21 22 23 24 25 26 27    20 21 22 23 24 25 26
24 25 26 27 28 29 30    28                      27 28 29 30 31      
31                                                                

4. To highlight the current date:

$ ncal -e

Output:

   September 2021
Su Mo Tu We Th Fr Sa
          1  2  3  4
 5  6  7  8 *9*10 11
12 13 14 15 16 17 18
19 20 21 22 23 24 25
26 27 28 29 30      

These are some examples of using the "ncal" command in different ways. 

## tldr 
 
> This command is an alias of `cal`.
> More information: <https://manned.org/ncal>.

- View documentation for the original command:

`tldr cal`
