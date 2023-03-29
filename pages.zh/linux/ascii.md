# ascii 
## chatgpt 
Linux命令ascii用于显示ASCII码表中的字符或者给定字符的ASCII码值。

使用该命令时，可以提供一个或多个以空格分隔的参数，每个参数为一个字符。这些字符可以是单个字符、转义序列（如\n、\r、\t等）或者十六进制表示的ASCII码值（如\x41表示A）。

如果没有提供参数，则ascii命令会打印完整的ASCII码表，包括ASCII码值和对应的字符。

例如，以下是使用ascii命令显示ASCII码表中数字0到9以及字母A到Z的输出：

```
$ ascii 0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ
  Oct   Dec   Hex   Char
  ---------------------------------
 060   48    0     0
 061   49    1     1
 062   50    2     2
 063   51    3     3
 064   52    4     4
 065   53    5     5
 066   54    6     6
 067   55    7     7
 070   56    8     8
 071   57    9     9
 101   65    41    A
 102   66    42    B
 103   67    43    C
 104   68    44    D
 105   69    45    E
 106   70    46    F
 107   71    47    G
 110   72    48    H
 111   73    49    I
 112   74    4A    J
 113   75    4B    K
 114   76    4C    L
 115   77    4D    M
 116   78    4E    N
 117   79    4F    O
 120   80    50    P
 121   81    51    Q
 122   82    52    R
 123   83    53    S
 124   84    54    T
 125   85    55    U
 126   86    56    V
 127   87    57    W
 130   88    58    X
 131   89    59    Y
 132   90    5A    Z
```

从上面的输出可以看出，ascii命令会打印每个字符的八进制（Oct）、十进制（Dec）和十六进制（Hex）表示，以及对应的ASCII字符（Char）。 

## tldr 
 
> 显示 ASCII 字符的别名。
> 更多信息：<http://www.catb.org/~esr/ascii/>.

- 显示一个 ASCII 字符的别名：

`ascii {{a}}`

- 以较短和脚本友好模式显示 ASCII 字符的别名：

`ascii -t {{a}}`

- 显示多个 ASCII 字符的别名：

`ascii -s {{tldr}}`

- 显示十进制 ASCII 字符表：

`ascii -d`

- 显示十六进制 ASCII 字符表：

`ascii -x`

- 显示八进制 ASCII 字符表：

`ascii -o`

- 显示二进制 ASCII 字符表：

`ascii -b`

- 显示选项总结和整个 ASCII 字符表：

`ascii`
