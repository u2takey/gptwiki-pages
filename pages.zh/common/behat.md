# behat 
## chatgpt 
behat是一个行为驱动测试(Behavior-Driven Development, BDD)框架，用于测试Web应用程序。

运行behat命令可以启动Behat测试，你需要提供要测试的特性文件的路径。特性文件是用于描述应用程序行为和期望输出的一个文件，通常使用Gherkin语言编写。

behat会读取特性文件中的测试场景，并执行这些场景的步骤。步骤可以是已经定义的步骤，也可以是需要定义的步骤。

behat还支持各种插件，可以扩展其功能。例如，可以添加Selenium插件，以使用Selenium WebDriver执行Web界面测试。

总之，运行behat命令是启动Behat测试的第一步，它会读取特性文件并执行测试场景。 

## tldr 
 
> 基于 Behaviour-Driven Development 的自动化测试 PHP 框架。
> 更多信息：<https://behat.org>.

- 初始化一个 PHP behat 项目：

`behat --init`

- 运行所有测试：

`behat`

- 运行指定组所有的测试用例：

`behat --suite={{组名}}`

- 运行所有测试，指定输入格式：

`behat --format {{pretty|progress}}`

- 将测试结果输出到指定文件：

`behat --out {{路径/到/文件}}`

- 展示测试组所在的目录清单：

`behat --definitions`
