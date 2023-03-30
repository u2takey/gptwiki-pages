# gshuf 
## chatgpt 
gshuf命令用于随机排列和选择输入的行。它在Linux和Unix系统中可用。

语法：

```
gshuf [OPTIONS] [FILE]
```

选项：

- -i，--input-range=ITEMS：从指定的范围中选择随机整数行。范围应用于逗号分隔的下限和上限。例如，-i 1-10,20-30。
- -n，--head-count=LINES：从输入的行中选取指定数量的行。
- -r，--repeat：允许在未选择的行中进行重复选择。
- -e，--echo：将输入的行包含在输出中，并添加随机选择的行。
- --help：显示帮助。

示例：

1. 从文件中选择5行，随机排序输出：

   ```
   gshuf -n 5 input.txt
   ```

2. 从1到20中选择5个不同的随机数：

   ```
   gshuf -i 1-20 -n 5
   ```

3. 从文件中进行重复选择：

   ```
   gshuf -r -n 5 input.txt
   ``` 

## tldr 
 
> 这是 `-p linux shuf` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux shuf`
