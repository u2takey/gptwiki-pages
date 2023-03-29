# case 
## chatgpt 
case命令是在shell脚本中进行多路分支选择的结构，类似于C语言中的switch语句。case语句由关键字case和esac（以反向拼写的case）包围。 先使用`case`指定要比较的变量，然后使用一个或多个分支，每个分支对应一个可能的值，并执行与该分支匹配的一系列命令。

语法：
```
case variable in
      pattern1)
            # commands to be executed
            ;;
      pattern2)
            # commands to be executed
            ;;
      ...
      patternN)
            # commands to be executed
            ;;
      *)
            # Default condition to be executed
            ;;
esac
```
在这里，variable可以是任何您想比较的值，而不仅仅是变量。模式可以是一个字符串，一个数字或一组数字，甚至是一个通配符。

这里有几个例子说明case命令的使用。

例1:
```
#!/bin/bash

echo "Enter the character: "
read char

case $char in
     [a-z] )
          echo "Character is lowercase alphabet."
          ;;
     [A-Z] )
          echo "Character is uppercase alphabet."
          ;;
     [0-9] )
          echo "Character is digit."
          ;;
     ? ) 
          echo "Character is special symbol."
          ;;
    * ) 
          echo "Unknown input."
          ;;
esac
```
这个例子将分别检查字符的小写字母，大写字母，数字和特殊字符。

例2：根据输入的日期格式推断出是星期几
```
#!/bin/bash

echo -n "Enter date (YYYY-MM-DD): "
read date

day=$(date -d"${date}" +%A)

case $day in
     Monday )
          echo "The day is Monday."
          ;;
     Tuesday )
          echo "The day is Tuesday."
          ;;
     Wednesday )
          echo "The day is Wednesday."
          ;;
     Thursday )
          echo "The day is Thursday."
          ;;
     Friday )
          echo "The day is Friday."
          ;;
    * ) 
          echo "The day is a weekend."
          ;;
esac
```
这个例子将具体检查输入日期是周一，周二，周三，周四，周五还是周末。
 

## tldr 
 
> case ... esac 与其他语言中的 switch ... case 语句类似，是一种多分枝选择结构。
> 更多信息：<https://manned.org/case>.

- 通过字符串字面量判断执行分支：

`case {{入参变量}} in {{字符字面量1}} {{执行语句块1}} ;; {{字符字面量2}}) {{执行语句块2}} ;; *) {{默认执行语句块}} ;; esac`

- 搭配通配符进行匹配，判断执行分支：

`case {{入参变量}} in {{通配符或者字符字面量}}) {{执行语句块1}} ; ;; {{通配符或者字符字面量}}) {{执行语句块1}}; ;; *) {{echo "what?"}}; ;; esac`
