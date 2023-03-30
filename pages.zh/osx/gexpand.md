# gexpand 
## chatgpt 
gexpand 是 GNU 工具包中的一个命令行工具，用于将宏定义展开为宏替换内容。以下是该命令的详细解释：

语法：

gexpand [选项] [输入文件] 

参数：

- [选项]：gexpand 可以接受以下选项：
    - -o, --output=<输出文件>：指定输出文件名。
    - -D, --define=<宏定义>：在展开时定义宏，多个定义用逗号隔开。
    - -U, --undefine=<宏名称>：在展开时取消定义的宏，多个名称用逗号隔开。
    - -C, --comprehend：在展开时进行条件编译。
    - -t, --tabs=<数字>：指定制表符的宽度。
    - -?, --help：显示 gexpand 的帮助信息。
    - --usage：显示 gexpand 命令的使用说明。
    - --version：显示 gexpand 的版本号。
- [输入文件]：需要进行宏展开的输入文件名。

工作原理：

gexpand 的工作原理如下：

1. 读入输入文件。
2. 将宏定义中的宏名及其替换文本存储到一个表中。
3. 扫描输入文件的每一行，找到其中的宏名，并将其替换为宏替换内容。
4. 输出展开后的结果到输出文件（如果指定了）或终端。

举例说明：

假设有以下 C 语言代码：

```
#define PI 3.14159
int main() {
    double r = 5.0;
    double area = PI * r * r;
    printf("The area of a circle with radius %lf is %lf.\n", r, area);
    return 0;
}
```

通过执行以下命令展开 PI 宏：

```
gexpand -D PI input.c
```

将得到以下展开后的代码：

```
int main() {
    double r = 5.0;
    double area = 3.14159 * r * r;
    printf("The area of a circle with radius %lf is %lf.\n", r, area);
    return 0;
}
``` 

## tldr 
 
> 这是 `-p linux expand` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux expand`
