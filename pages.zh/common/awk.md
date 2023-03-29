# awk 
## chatgpt 
awk是一种文本处理工具，是一个强大的通用脚本语言，由美国贝尔实验室的Al Aho、Peter Weinberger和Brian Kernighan于1977年推出。它可以读取文本文件、处理数据、筛选信息并生成报告。它的名字得自于它的三位发明者的姓氏的首字母。

awk的使用是通过编写一个执行特定任务的脚本程序来完成。这个脚本程序从awk程序的输入文件中读取数据，对这些数据进行处理，然后将处理结果写入标准输出或输出到其他数据文件中。

awk程序是由一系列模式和命令构成的。模式即是用于匹配输入数据的模式，而命令则是对匹配到的数据进行处理的操作。awk程序对每一行数据都会执行这些模式和命令，从而对整个文件或者数据流进行处理。 

awk命令的语法如下：

```bash
awk [options] 'pattern {action}' file
```

其中，options是awk命令的可选参数，pattern是awk程序的匹配模式，action是匹配到模式时要执行的一系列命令，file是待处理的数据文件。

使用awk命令可以实现很多文本处理的功能，例如：

- 选取某些列
- 搜索匹配某些条件的行
- 对数据进行计算处理
- 将数据格式化输出

以下是一些常用的awk命令：

```bash
# 选取某些列
awk '{print $1}' file                    # 输出文件的第一列
awk '{print $1, $3}' file                # 输出文件的第一列和第三列
awk -F':' '{print $1,$3}' /etc/passwd    # 以冒号分隔符分隔文件，并输出文件的第一列和第三列

# 搜索匹配某些条件的行
awk '/pattern/' file                      # 输出文件中包含pattern的行
awk '{if ($1=="keyword") print $0}' file  # 输出文件中第一列为keyword的行
awk '$1=="keyword" {print $0}' file       # 输出文件中第一列为keyword的行

# 对数据进行计算处理
awk '{sum+=$1} END{print sum}' file       # 计算文件中第一列的总和并输出
awk '{avg+=$1; count+=1} END{print avg/count}' file  # 计算文件中第一列的平均值并输出
awk '{print $1*3, $2+10}' file            # 对文件中的第一列乘以3，第二列加上10，全部输出

# 将数据格式化输出
awk '{printf "%-8s %-10s\n", $1, $2}' file  # 左对齐输出文件的第一列和第二列
``` 

## tldr 
 
> 一种用于文件处理的通用编程语言。
> 更多信息：<https://github.com/onetrueawk/awk>.

- 以空格为分隔符，打印文件每行第五列（也称作字段）：

`awk '{print $5}' {{文件名}}`

- 以空格为分隔符，打印文件包含“foo” 的所有行的第二列：

`awk '/{{foo}}/ {print $2}' {{文件名}}`

- 以逗号而不是空格作为分隔符，打印文件每行的最后一列：

`awk -F ',' '{print $NF}' {{文件名}}`

- 计算文件的第一列数值之和并打印：

`awk '{s+=$1} END {print s}' {{文件名}}`

- 从第一行开始，每三行打印一行：

`awk 'NR%3==1' {{文件名}}`

- 根据条件不同，打印不同内容：

`awk '{if ($1 == "foo") print "Exact match foo"; else if ($1 ~ "bar") print "Partial match bar"; else print "Baz"}' {{文件名}}`

- 打印第 10 列等于指定值的所有行：

`awk '($10 == 指定值)'`

- 打印第 10 列介于最小值和最大值之间的所有行：

`awk '($10 >= 最小值 && $10 <= 最大值)'`
