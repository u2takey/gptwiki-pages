#grep 
## chatgpt 
grep命令是一个文本搜索工具，用于在指定的文件中查找符合用户指定模式的文本行，并将该行文本输出到屏幕。

常见用法：

1. grep pattern filename：在filename文件中查找包含pattern的行。

2. grep -r pattern directory：在directory目录及其子目录中查找包含pattern的行。

3. grep -v pattern filename：在filename文件中查找不包含pattern的行。

4. grep -i pattern filename：在filename文件中查找包含pattern的行，不区分大小写。

5. grep -c pattern filename：在filename文件中查找包含pattern的行，并统计出现次数。

6. grep -n pattern filename：在filename文件中查找包含pattern的行，并显示行号。

7. grep -E or egrep pattern filename：使用扩展正则表达式在filename文件中查找包含pattern的行。

8. grep -f pattern_file filename：在filename文件中查找与pattern_file文件中所有模式匹配的行。

9. grep -l pattern filename：在filename文件中查找包含pattern的行，并输出符合条件的文件名。

10. grep -L pattern filename：在filename文件中查找不包含pattern的行，并输出符合条件的文件名。