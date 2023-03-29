# vim 
## chatgpt 
vim是一个文本编辑器，它可以在Linux、Unix、macOS和Windows等操作系统中使用。它可以用于编辑各种类型的文本文件，如代码、配置文件和文本文档等。

下面是一些常用的vim命令及其作用：

1. 打开/创建文件：vim filename

2. 退出vim编辑器：

   :q ：退出（若修改过文本则提示保存）

   :w ：保存当前编辑的文本

   :wq ：保存并退出编辑器

   :q! ：强制退出，放弃所有修改

3. 光标移动：

   h：左移光标

   j：下移光标

   k：上移光标

   l：右移光标

   组合使用：

   w：向右移动一个单词

   b：向左移动一个单词

   $：移动到行尾

   0：移动到行首

   G：移动到文件末尾

   gg：移动到文件开头

4. 文本编辑：

   i：在当前光标位置插入文本

   a：在光标下一个位置插入文本

   o：在当前行下面添加新行并插入文本

   O：在当前行上面添加新行并插入文本

   x：删除当前光标所在位置的字符

   r：替换当前光标所在位置的字符

   u：撤销最后一次编辑

   Ctrl+r：恢复最后一次撤销的操作

5. 搜索替换：

   /text：在当前文件中查找text（n：下一个匹配，N：上一个匹配）

   :s/old/new/g：将当前行中的old替换为new（可加%表示整个文本）

   :%s/old/new/gc：将整个文本中的old替换为new，并逐个确认是否要替换（c表示确认）

6. 其他命令：

   :set number：显示行号

   :set nonumber：隐藏行号

   :set autoindent：自动缩进

   :set tabstop=4：设置Tab键宽度为4个空格

   :set list：显示不可见字符

   :set ai：自动缩进

   :set incsearch：搜索时逐步显示匹配项

这些命令只是vim命令的冰山一角，vim有着丰富的命令和插件，可以让你在编辑文本时更加高效。 

## tldr 
 
> Vi IMproved，一个程序员的文本编辑器，提供为不同类型的文档修改设计的多种模式。
> 按 `i` 进入插入模式。`<Esc>` 返回正常模式，正常模式允许使用 Vim 命令。
> 更多信息：<https://www.vim.org>.

- 打开文档：

`vim {{文件}}`

- 打开文件的指定行数：

`vim +{{行数}} {{文件}}`

- 查看 Vim 的使用说明：

`:help<Enter>`

- 保存并退出：

`:wq<Enter>`

- 撤销上一个操作：

`u`

- 用特征（pattern）在文件中搜寻，按下 `n`/`N` 切换至上 / 下一个结果：

`/{{特征}}<Enter>`

- 对整个文件使用正则表达式进行替换：

`:%s/{{正则表达式}}/{{替换字}}/g<Enter>`

- 显示行号：

`:set nu<Enter>`